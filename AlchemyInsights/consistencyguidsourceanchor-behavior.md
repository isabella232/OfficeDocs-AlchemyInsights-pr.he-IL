---
title: התנהגות ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705734"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>התנהגות ConsistencyGuid/sourceAnchor

תכלת התחברות (גירסה 1.1.524.0 ולאחר) כעת מקלה על השימוש ב-msDS-ConsistencyGuid כתכונה sourceAnchor. בעת השימוש בתכונה זו, ' התכלת התחברות ' מגדירה באופן אוטומטי את כללי הסנכרון ל:
  
- השתמש ב-msDS-ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש. ObjectGUID משמש עבור סוגי אובייקטים אחרים.
    
- עבור כל אובייקט משתמש מקומי נתון שהתכונה msDS-ConsistencyGuid שלו אינה מאוכלסת, התכונה התכלת לספירה כותבת את ערך objectGUID בחזרה לתכונת msDS-ConsistencyGuid ב-Active Directory המקומי. לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, הכלי התכלת התחבר לאחר מכן מייצא את האובייקט לתכלת.
    
 **הערה:** לאחר ייבוא של אובייקט AD מקומי לתוך התכלת (כלומר, מיובא לתוך שטח המחבר של AD ומוקרן לתוך מטברס), אין באפשרותך לשנות יותר את ערך ה-sourceAnchor שלו. כדי לציין את ערך sourceAnchor עבור אובייקט AD מקומי נתון, הגדר את התכונה msDS-ConsistencyGuid שלו לפני שתיובא לתוך החיבור לתכלת. 
  
לקבלת מידע נוסף על SourceAnchor ו-ConsistencyGuid, עיין בפרטים הבאים: [תכלת חיבור: מושגים בעיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

