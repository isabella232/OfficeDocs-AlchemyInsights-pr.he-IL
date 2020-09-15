---
title: מפתחות שחזור של Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685887"
---
# <a name="accessing-bitlocker-recovery-keys"></a>גישה למפתחות שחזור של Bitlocker

בעת קביעת התצורה של מדיניות הגנת נקודות הקצה של Bitlocker, ניתן להגדיר אם יש לאחסן את מידע השחזור של Bitlocker ב-תכלת Active Directory.

אם הגדרה זו מוגדרת, נתוני השחזור המאוחסנים אמורים להיות גלויים לניהול מכוונן כחלק מנתוני רשומת ההתקן בלהב של התקנים מובילים בשתי דרכים:

מכשירים-תכלת מכשירים-> "Device" או מכשירים-> כל המכשירים-> "התקן"-מפתחות שחזור >

לחלופין, אם קיימת גישה מנהלית למכשיר עצמו, ניתן לראות את מפתח השחזור (סיסמה) על-ידי הפעלת הפקודה הבאה מתוך שורת פקודה מוגבהת:

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
אם המכשיר הוצפן לפני רישום בתוך המנגינה, ייתכן שמפתח השחזור השויך ל-"Microsoft Account" (ולכת למס א) המשמש לכניסה למכשיר במהלך תהליך ה-OOBE. אם זה היה המקרה, כניסה  https://onedrive.live.com/recoverykey וכניסה באמצעות ולכת למס א אמור להראות את המכשירים שעבורם אוחסנו מפתחות השחזור.
 
אם המכשיר הוצפן כתוצאה מקביעת תצורה באמצעות מדיניות קבוצתית מבוססת תחום, מידע השחזור עשוי להיות מאוחסן ב-Active Directory המקומי.
 

