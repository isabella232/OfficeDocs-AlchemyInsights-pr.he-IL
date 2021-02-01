---
title: בעיות באישורים
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063630"
---
# <a name="issues-with-credentials"></a>בעיות באישורים

[פלטפורמת הזהויות של Microsoft וזרימת אישורי הלקוח של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) מתארת כיצד לתכנת ישירות מול אישורי הלקוח של OAuth 2.0 מעניקים זרימה.

**כיצד ניתן לנהל את הסיסמה או אישורי האישור של היישום?**

ב-תכלת CLI, באפשרותך להשתמש [באישור האפליקציה az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) כדי למחוק, לפרט או לאפס את הסיסמה או אישורי האישור של היישום.

**כיצד המשתמשים שלי מאפסים את הסיסמאות שלהם?**

המשתמשים צריכים [להירשם לאיפוס סיסמה בשירות עצמי](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) לפני שיוכלו לאפס את הסיסמאות שלהם. לאחר שמשתמש נרשם, הם יכולים לבצע את ההוראות במאמר זה כדי לאפס את הסיסמה שלו: [לאפס את הסיסמה שלך בעבודה או בבית הספר](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**כיצד המשתמשים שלי משנים את הסיסמאות שלהם?**

המשתמשים יכולים לבצע את השלבים המפורטים במאמר זה כדי לשנות את הסיסמאות שלהם: [כיצד לשנות את הסיסמה שלך](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
הם יכולים גם [לנהל סיסמאות של יישומים עבור אימות של שני שלבים](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**המשתמש שלי מקבל שגיאה בעת שינוי או איפוס של הסיסמה שלו**

קישור זה יספק מידע על בעיות נפוצות שעלולות להתעורר כאשר משתמש מנסה לאפס את הסיסמה שלו: [בעיות נפוצות והפתרונות שלהם](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**אני נתקל בבעיה באיפוס סיסמת משתמש**

- ודא שאתה מורשה לאפס סיסמאות. *רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.* מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.

- ודא שהבנת את דרישות הרישוי:

  - דרוש לך רשיון אחד לפחות שהוקצה בארגון שלך:
    - **משתמשים בענן בלבד** -כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic
    - **משתמשים בענן ו/או מקומיים** -תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)
    - לקבלת מידע נוסף על דרישות הרישוי, ראה [דרישות רישוי עבור איפוס סיסמה בשירות עצמי של תכלת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- כדי לאפס סיסמת משתמש, אתר את המשתמש בתכלת לספירה. לאחר מכן, בלהב מבט כולל עבור משתמש זה, לחץ על לחצן ' איפוס סיסמה '.

**לחצן ' איפוס סיסמה ' מופיע באפור**

אין לך הרשאה לאפס את הסיסמאות של משתמש **זה** . *רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.* מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.

**איני רואה את להב איפוס הסיסמה**

אין לך הרשאה לאפס סיסמאות. *רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.* מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.

**איני רואה את להב השילוב המקומי באיפוס סיסמה**

- להב השילוב המקומי מופיע רק בסביבות היברידיות-כלומר, אתה משתמש ב-writeback password כדי לטפל בסיסמאות של משתמש מקומי.

- אינך רואה את הלהב הזה אם:

  - אינך משתמש ב-password writeback
  - קיימת בעיה בהתקנה/בקישוריות של writeback סיסמה
  - קיימת בעיה בהתקנה/בקישוריות של התחברות של תכלת לספירה
  - לקבלת שלבים נוספים לפתרון בעיות בנושא בעיות בwriteback סיסמאות, ראה [פתרון בעיות בסיסמאות writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**איני יודע כיצד לאפס סיסמת משתמש**

1. היכנס לפורטל ' תכלת ' כמנהל מתאים.
2. עבור אל הלהב **משתמשים וקבוצות** , בחר **את כל המשתמשים**.
3. בחר משתמש מהרשימה.
4. עבור המשתמש שנבחר, בחר **מבט כולל** ולאחר מכן, בסרגל הפקודות, בחר **איפוס סיסמה**.
5. בחר בלחצן **אפס סיסמה** ובצע את ההוראות המופיעות על המסך.
    - רק איפוסים שבוצעו באמצעות הסיסמה ' תמיכה **בפורטל** של writeback '.

**אני מאפס סיסמה של משתמש מקומי מפורטל הניהול של Office 365 או מהיישום Office 365 למכשירים ניידים, אך המשתמש עדיין אינו מצליח להיכנס**

Writeback סיסמה אינו נתמך בפורטל זה. אפס את סיסמת המשתמש שוב בפורטל התכלת.
