---
title: ConsistencyGuid / sourceAnchor התנהגות
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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408109"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor התנהגות

התחבר AD תכלת הרקיע (גירסה 1.1.524.0 ואחרי) כעת מקל את השימוש msDS ConsistencyGuid כתכונה sourceAnchor. בעת שימוש בתכונה זו, התחבר AD תכלת הרקיע מגדירה באופן אוטומטי את הכללים סינכרון:
  
- השתמש msDS ConsistencyGuid כתכונה sourceAnchor עבור אובייקטי משתמש. ObjectGUID משמש עבור סוגים אחרים של אובייקט.
    
- עבור כל נתון המקומית משתמש AD האובייקט שאת תכונת msDS ConsistencyGuid לא יכתוב התחבר AD שהוכנה, תכלת הרקיע ערכו objectGUID בחזרה התכונה msDS ConsistencyGuid ב- Active Directory מקומי. לאחר מאוכלס התכונה msDS ConsistencyGuid, התחבר AD תכלת הרקיע מכן ייצוא האובייקט AD תכלת הרקיע.
    
 **הערה:** פעם אחת מקומי AD אובייקט מיובא לתוך התחבר AD תכלת הרקיע (כלומר, מיובאים לתוך הרווח מחבר AD ו מתוכנן לתוך ה-Metaverse), אין באפשרותך לשנות את הערך sourceAnchor שלו עוד. כדי לציין את הערך sourceAnchor עבור בהינתן המקומית AD אובייקט, קביעת תצורה של תכונה msDS ConsistencyGuid שלו לפני הוא מיובא לתוך התחבר AD תכלת הרקיע. 
  
לקבלת מידע נוסף אודות SourceAnchor ו- ConsistencyGuid, התייחס לנושאים הבאים: [התחבר AD תכלת הרקיע: עיצוב מושגים](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

