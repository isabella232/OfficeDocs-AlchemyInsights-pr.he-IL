---
title: אין אפשרות להגדיר או להציג את המדיניות ' אפשר שירותרכישה '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091710"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>אין אפשרות להגדיר או להציג את המדיניות ' אפשר שירותרכישה '

בעת ניסיון להגדיר או להציג את המדיניות אפשר שירות הרכישה, מתקבלת הודעת השגיאה הבאה:

*שגיאת התקשרות: לא היתה אפשרות לאחזר מדיניות מוצר עם מזהה שירות ' אפשר שירותרכישה ', הודעת שגיאה-החיבור הבסיסי נסגר: אירעה שגיאה בלתי צפויה בשליחה.*

ייתכן שהסיבה לכך היא גירסה ישנה יותר של אבטחת שכבת התעבורה (TLS). כדי לחבר את שירות MSCommerce, עליך להשתמש ב-TLS 1.2 או בגדול יותר.  

נסה את השלבים הבאים כדי להפעיל/להגדיר את פרוטוקול TLS ל1.2, לאמת ולנסות שנית.
 1. בשורת הפקודה PowerShell (PS C:\) הזן את הפקודה הבאה כדי להגדיר את פרוטוקול TLS לגירסה 1.2:

    \[Net. שירותי מנהל הרשת:: פרוטוקול \[אבטחה = Net. אבטחה פרוטוקולטיפ]:: Tls12

2. אמת את הפרוטוקולים של TLS בשימוש, עם הפקודה הבאה:

    \[מנהל הרשת:: פרוטוקול אבטחה 

3. נסה שוב את הפקודות קבל או עדכן לפי הצורך.

