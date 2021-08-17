---
title: מפתחות שחזור של Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060065"
---
# <a name="accessing-bitlocker-recovery-keys"></a>גישה למפתחות שחזור של Bitlocker

בעת קביעת התצורה של הגדרות Bitlocker Intune Endpoint Protection מדיניות, ניתן להגדיר אם יש לאחסן מידע שחזור של Bitlocker ב- Azure Active Directory.

אם הגדרה זו מוגדרת, נתוני השחזור המאוחסנים אמורים להיות גלויים למנהל Intune כחלק מנתוני הרשומה של המכשיר בלהב Intune Devices בשתי דרכים:

מכשירים - מכשירי Azure AD -> "Device" OR Devices -> כל המכשירים -> "Device" -> מפתחות שחזור

לחלופין, אם ישנה גישה ניהולית למכשיר עצמו, ניתן לראות את מפתח השחזור (סיסמה) על-ידי הפעלת הפקודה הבאה משורת פקודה עם הרשאות מלאות:

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
אם המכשיר הוצפן לפני הרישום ב- Intune, ייתכן שמפתח השחזור משויך ל-"Microsoft Account" (MSA) ששימש כדי להיכנס למכשיר במהלך תהליך ה- OOBE. במקרה זה, הגישה וההכניסה באמצעות MSA זה אמורים  https://onedrive.live.com/recoverykey להציג את המכשירים שעבורם אוחסנו מפתחות שחזור.
 
אם המכשיר היה מוצפן כתוצאה מתצורה באמצעות מדיניות קבוצתית מבוססת תחום, ייתכן שמידע השחזור יאוחסן ב- Active Directory המקומי.

אם הגדרת מדיניות הגנה על נקודת קצה לאחסון מפתח השחזור ב- Azure Active Directory, אך המפתח עבור מכשיר ספציפי לא הועלה, באפשרותך להפעיל את ההעלאה על-ידי סיבוב מפתח השחזור עבור מכשיר זה ממסוף MEM. לקבלת פרטים, ראה [סיבוב מפתחות שחזור של BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

