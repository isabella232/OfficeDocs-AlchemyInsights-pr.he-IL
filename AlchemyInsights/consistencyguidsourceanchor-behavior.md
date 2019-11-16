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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516983"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>התנהגות ConsistencyGuid/sourceAnchor

תכלת התחברות (גירסה 1.1.524.0 ולאחר) כעת מקלה על השימוש ב-msDS-ConsistencyGuid כתכונה sourceAnchor. בעת השימוש בתכונה זו, ' התכלת התחברות ' מגדירה באופן אוטומטי את כללי הסנכרון ל:
  
- השתמש ב-msDS-ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש. ObjectGUID משמש עבור סוגי אובייקטים אחרים.
    
- עבור כל אובייקט משתמש מקומי נתון שהתכונה msDS-ConsistencyGuid שלו אינה מאוכלסת, התכונה התכלת לספירה כותבת את ערך objectGUID בחזרה לתכונת msDS-ConsistencyGuid ב-Active Directory המקומי. לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, הכלי התכלת התחבר לאחר מכן מייצא את האובייקט לתכלת.
    
 **הערה:** לאחר ייבוא של אובייקט AD מקומי לתוך התכלת (כלומר, מיובא לתוך שטח המחבר של AD ומוקרן לתוך מטברס), אין באפשרותך לשנות יותר את ערך ה-sourceAnchor שלו. כדי לציין את ערך sourceAnchor עבור אובייקט AD מקומי נתון, הגדר את התכונה msDS-ConsistencyGuid שלו לפני שתיובא לתוך החיבור לתכלת. 
  
לקבלת מידע נוסף על SourceAnchor ו-ConsistencyGuid, עיין בפרטים הבאים: [תכלת חיבור: מושגים בעיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

