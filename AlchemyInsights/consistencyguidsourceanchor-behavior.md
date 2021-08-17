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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044341"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>עקביותGuid / sourceAnchor behavior

Azure AD התחברות (גירסה 1.1.524.0 ולאחר) מקלה כעת על השימוש בתכונה msDS-ConsistencyGuid כתכונה sourceAnchor. בעת שימוש בתכונה זו, Azure AD התחברות באופן אוטומטי את כללי הסינכרון כך:
  
- השתמש ב- msDS-ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש. ObjectGUID משמש עבור סוגי אובייקטים אחרים.
    
- עבור כל אובייקט נתון מקומי של משתמש AD שהתכונה msDS-ConsistencyGuid שלו אינה מאוכלסת, Azure AD התחברות כותב את ערך objectGUID שלו בחזרה לתכונה msDS-ConsistencyGuid ב- Active Directory המקומי. לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, Azure AD התחברות מכן מייצא את האובייקט ל- Azure AD.
    
 **הערה:** לאחר ייבוא אובייקט AD מקומי ל- Azure AD התחברות (שהוא, מיובא למרחב המחבר של AD ומופרין לתוך Metaverse), לא ניתן לשנות את ערך sourceAnchor שלו עוד. כדי לציין את הערך sourceAnchor עבור אובייקט AD מקומי נתון, הגדר את התכונה msDS-ConsistencyGuid שלו לפני ייבואו ל- Azure AD התחברות. 
  
לקבלת מידע נוסף אודות SourceAnchor ו- ConsistencyGuid, עיין במאמרים הבאים: [Azure AD התחברות: מושגי עיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

