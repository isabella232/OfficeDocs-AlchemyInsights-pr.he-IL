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
# <a name="consistencyguid--sourceanchor-behavior"></a>עקביותGuid / sourceAnchor behavior

Azure AD Connect (גירסה 1.1.524.0 ולאחר) מקל כעת על השימוש בתכונה msDS-ConsistencyGuid כתכונה sourceAnchor. בעת שימוש בתכונה זו, Azure AD Connect מגדיר באופן אוטומטי את כללי הסינכרון כך:
  
- השתמש ב- msDS-ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש. ObjectGUID משמש עבור סוגי אובייקטים אחרים.
    
- עבור כל אובייקט נתון מקומי של משתמש AD שהתכונה msDS-ConsistencyGuid שלו אינה מאוכלסת, Azure AD Connect כותב את ערך OBJECTGUID שלו בחזרה לתכונה msDS-ConsistencyGuid ב- Active Directory המקומי. לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, Azure AD Connect מייצא את האובייקט ל- Azure AD.
    
 **הערה:** לאחר ייבוא אובייקט AD מקומי ל- Azure AD Connect (שהוא, מיובא למרחב המחבר של AD ומופרק ל- Metaverse), לא ניתן לשנות את ערך sourceAnchor שלו עוד. כדי לציין את הערך sourceAnchor עבור אובייקט AD מקומי נתון, קבע את תצורת התכונה msDS-ConsistencyGuid שלו לפני ייבואו ל- Azure AD Connect. 
  
לקבלת מידע נוסף אודות SourceAnchor ו- ConsistencyGuid, עיין בנושאים הבאים: [Azure AD Connect: מושגי עיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

