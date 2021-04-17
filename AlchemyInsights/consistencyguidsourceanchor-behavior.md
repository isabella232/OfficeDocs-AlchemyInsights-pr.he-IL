---
title: עקביותGuid / sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816993"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="6a63f-102">עקביותGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="6a63f-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="6a63f-103">Azure AD Connect (גירסה 1.1.524.0 ולאחר) מקל כעת על השימוש בתכונה msDS-ConsistencyGuid כתכונה sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="6a63f-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="6a63f-104">בעת שימוש בתכונה זו, Azure AD Connect מגדיר באופן אוטומטי את כללי הסינכרון כך:</span><span class="sxs-lookup"><span data-stu-id="6a63f-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="6a63f-105">השתמש ב- msDS-ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש.</span><span class="sxs-lookup"><span data-stu-id="6a63f-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="6a63f-106">ObjectGUID משמש עבור סוגי אובייקטים אחרים.</span><span class="sxs-lookup"><span data-stu-id="6a63f-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="6a63f-107">עבור כל אובייקט נתון מקומי של משתמש AD שהתכונה msDS-ConsistencyGuid שלו אינה מאוכלסת, Azure AD Connect כותב את ערך OBJECTGUID שלו בחזרה לתכונה msDS-ConsistencyGuid ב- Active Directory המקומי.</span><span class="sxs-lookup"><span data-stu-id="6a63f-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="6a63f-108">לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, Azure AD Connect מייצא את האובייקט ל- Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6a63f-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="6a63f-109">**הערה:** לאחר ייבוא אובייקט AD מקומי ל- Azure AD Connect (שהוא, מיובא למרחב המחבר של AD ומופרק ל- Metaverse), לא ניתן לשנות את ערך sourceAnchor שלו עוד.</span><span class="sxs-lookup"><span data-stu-id="6a63f-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="6a63f-110">כדי לציין את הערך sourceAnchor עבור אובייקט AD מקומי נתון, קבע את תצורת התכונה msDS-ConsistencyGuid שלו לפני ייבואו ל- Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6a63f-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="6a63f-111">לקבלת מידע נוסף אודות SourceAnchor ו- ConsistencyGuid, עיין בנושאים הבאים: [Azure AD Connect: מושגי עיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="6a63f-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

