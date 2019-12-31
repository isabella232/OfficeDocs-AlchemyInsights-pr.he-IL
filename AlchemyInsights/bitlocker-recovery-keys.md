---
title: מפתחות שחזור של Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908816"
---
# <a name="accessing-bitlocker-recovery-keys"></a>גישה למפתחות שחזור של Bitlocker

בעת קביעת התצורה של הגדרות Bitlocker Intune מדיניות הגנת נקודות קצה, ניתן להגדיר אם יש לאחסן מידע שחזור של Bitlocker בתיקיה ' פעיל '.

אם תצורתה של הגדרה זו נקבעת, על נתוני השחזור המאוחסנים להיות גלויים למנהל Intune כחלק מנתוני רשומת ההתקן בלהב Intune Devices בשתי דרכים:

התקנים-התקנים לספירה למעלה-התקן או התקנים-מכשירים/התקנים מבוססי-_ gt_ כל ההתקנים-_ Gt_ "התקן"-_ Gt_ מפתחות שחזור

לחילופין, אם יש גישה ניהולית להתקן עצמו, ניתן לראות את מפתח השחזור (Password) על-ידי הפעלת הפקודה הבאה משורת פקודה מוגבהת:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
אם ההתקן הוצפן לפני רישום ב-Intune, ייתכן שמפתח השחזור השויך ל-"חשבון Microsoft" (מס א) ששימש לכניסה להתקן במהלך תהליך ה-OOBE. אם זה היה המקרה, גישה https://onedrive.live.com/recoverykey וכניסה עם זה מס ' מס צריך להראות את המכשירים שבהם אוחסנו מפתחות שחזור.
 
אם ההתקן הוצפן כתוצאה מתצורה באמצעות מדיניות קבוצתית מבוססת-תחום, ייתכן שמידע השחזור יאוחסן בספריה המקומית של Active Directory.
 

