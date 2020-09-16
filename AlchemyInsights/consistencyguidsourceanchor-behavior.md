---
title: התנהגות ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756284"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b3848-102">התנהגות ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="b3848-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b3848-103">התחברות למודעת תכלת (גירסה 1.1.524.0 ואחרי) מסייעת כעת לשימוש ב-msDS-ConsistencyGuid כתכונה sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="b3848-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b3848-104">בעת שימוש בתכונה זו, התכונה ' תכלת לספירה ' מגדירה באופן אוטומטי את כללי הסינכרון ל:</span><span class="sxs-lookup"><span data-stu-id="b3848-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b3848-105">השתמש ב-msDS-ConsistencyGuid כתכונה של sourceAnchor עבור אובייקטי משתמשים.</span><span class="sxs-lookup"><span data-stu-id="b3848-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b3848-106">ObjectGUID משמש עבור סוגי אובייקטים אחרים.</span><span class="sxs-lookup"><span data-stu-id="b3848-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b3848-107">עבור כל אובייקט מקומי נתון של AD מקומי שהתכונה msDS-ConsistencyGuid אינה מאוכלסת, הקישור תכלת AD כותב את ערך objectGUID בחזרה לתכונה msDS-ConsistencyGuid ב-Active Directory מקומי.</span><span class="sxs-lookup"><span data-stu-id="b3848-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b3848-108">לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, האפשרות תכלת AD Connect ולאחר מכן מייצאת את האובייקט לכיוון תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="b3848-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b3848-109">**הערה:** לאחר הייבוא של אובייקט AD מקומי לחיבור הודעות מיידיות (כלומר, המיובא לשטח מחבר המודעה ומוקרן לתוך Metaverse), אין באפשרותך לשנות את הערך של sourceAnchor עוד.</span><span class="sxs-lookup"><span data-stu-id="b3848-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b3848-110">כדי לציין את הערך של sourceAnchor עבור אובייקט AD מקומי נתון, קבע את תצורת התכונה msDS-ConsistencyGuid לפני הייבוא לתוך הקישור תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="b3848-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b3848-111">לקבלת מידע נוסף אודות SourceAnchor ו-ConsistencyGuid, עיין במאמר הבא: [מושגי החיבור של תכלת לספירה: מושגי עיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b3848-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

