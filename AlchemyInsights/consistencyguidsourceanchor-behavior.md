---
title: ConsistencyGuid / sourceAnchor התנהגות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659592"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3fcbb-102">ConsistencyGuid / sourceAnchor התנהגות</span><span class="sxs-lookup"><span data-stu-id="3fcbb-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3fcbb-p101">התחבר AD תכלת הרקיע (גירסה 1.1.524.0 ואחרי) כעת מקל את השימוש msDS ConsistencyGuid כתכונה sourceAnchor. בעת שימוש בתכונה זו, התחבר AD תכלת הרקיע מגדירה באופן אוטומטי את הכללים סינכרון:</span><span class="sxs-lookup"><span data-stu-id="3fcbb-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3fcbb-p102">השתמש msDS ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש. ObjectGUID משמש עבור סוגים אחרים של אובייקט.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3fcbb-p103">עבור כל נתון המקומית משתמש AD האובייקט שאת תכונת msDS ConsistencyGuid לא יכתוב התחבר AD שהוכנה, תכלת הרקיע ערכו objectGUID בחזרה התכונה msDS ConsistencyGuid ב- Active Directory מקומי. לאחר מאוכלס התכונה msDS ConsistencyGuid, התחבר AD תכלת הרקיע מכן ייצוא האובייקט AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3fcbb-p104">**הערה:** פעם אחת מקומי AD אובייקט מיובא לתוך התחבר AD תכלת הרקיע (כלומר, מיובאים לתוך הרווח מחבר AD ו מתוכנן לתוך ה-Metaverse), אין באפשרותך לשנות את הערך sourceAnchor שלו עוד. כדי לציין את הערך sourceAnchor עבור בהינתן המקומית AD אובייקט, קביעת תצורה של תכונה msDS ConsistencyGuid שלו לפני הוא מיובא לתוך התחבר AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3fcbb-111">לקבלת מידע נוסף אודות SourceAnchor ו- ConsistencyGuid, התייחס לנושאים הבאים: [התחבר AD תכלת הרקיע: עיצוב מושגים](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3fcbb-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

