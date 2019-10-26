---
title: התנהגות ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36516983"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="8f31e-102">התנהגות ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="8f31e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="8f31e-103">תכלת התחברות (גירסה 1.1.524.0 ולאחר) כעת מקלה על השימוש ב-msDS-ConsistencyGuid כתכונה sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="8f31e-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="8f31e-104">בעת השימוש בתכונה זו, ' התכלת התחברות ' מגדירה באופן אוטומטי את כללי הסנכרון ל:</span><span class="sxs-lookup"><span data-stu-id="8f31e-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="8f31e-105">השתמש ב-msDS-ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש.</span><span class="sxs-lookup"><span data-stu-id="8f31e-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="8f31e-106">ObjectGUID משמש עבור סוגי אובייקטים אחרים.</span><span class="sxs-lookup"><span data-stu-id="8f31e-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="8f31e-107">עבור כל אובייקט משתמש מקומי נתון שהתכונה msDS-ConsistencyGuid שלו אינה מאוכלסת, התכונה התכלת לספירה כותבת את ערך objectGUID בחזרה לתכונת msDS-ConsistencyGuid ב-Active Directory המקומי.</span><span class="sxs-lookup"><span data-stu-id="8f31e-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="8f31e-108">לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, הכלי התכלת התחבר לאחר מכן מייצא את האובייקט לתכלת.</span><span class="sxs-lookup"><span data-stu-id="8f31e-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="8f31e-109">**הערה:** לאחר ייבוא של אובייקט AD מקומי לתוך התכלת (כלומר, מיובא לתוך שטח המחבר של AD ומוקרן לתוך מטברס), אין באפשרותך לשנות יותר את ערך ה-sourceAnchor שלו.</span><span class="sxs-lookup"><span data-stu-id="8f31e-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="8f31e-110">כדי לציין את ערך sourceAnchor עבור אובייקט AD מקומי נתון, הגדר את התכונה msDS-ConsistencyGuid שלו לפני שתיובא לתוך החיבור לתכלת.</span><span class="sxs-lookup"><span data-stu-id="8f31e-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="8f31e-111">לקבלת מידע נוסף על SourceAnchor ו-ConsistencyGuid, עיין בפרטים הבאים: [תכלת חיבור: מושגים בעיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="8f31e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

