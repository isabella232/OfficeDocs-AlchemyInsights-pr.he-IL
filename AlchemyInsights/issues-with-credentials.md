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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986820"
---
# <a name="issues-with-credentials"></a>בעיות באישורים

[פלטפורמת הזהויות של Microsoft אישורי לקוח של OAuth 2.0 מתארים](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) כיצד לתכנת ישירות מול אישורי הלקוח OAuth 2.0 להעניק זרימה.

**כיצד ניתן לנהל סיסמה או אישורי אישור של יישום?**

ב- Azure CLI, באפשרותך להשתמש [באישורי אפליקציית az](https://docs.microsoft.com/cli/azure/ad/app/credential) כדי למחוק, רשימה או לאפס את הסיסמה או אישורי האישורים של יישום.

**כיצד המשתמשים שלי לאפס את הסיסמאות שלהם?**

המשתמשים צריכים [להירשם לאיפוס סיסמה בשירות עצמי](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) כדי שהם יוכלו לאפס את הסיסמאות שלהם. לאחר שמשתמש נרשם, הוא יכול לבצע את ההוראות במאמר זה כדי לאפס את הסיסמה שלו: איפוס [סיסמת העבודה או בית הספר.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**כיצד המשתמשים שלי לשנות את הסיסמאות שלהם?**

משתמשים יכולים לבצע את השלבים המפורטים במאמר זה כדי לשנות את הסיסמאות שלהם: [כיצד לשנות את הסיסמה שלך.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
הם יכולים גם [לנהל סיסמאות אפליקציה לאימות דו-שלבי.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**המשתמש שלי מקבל שגיאה בעת שינוי או איפוס הסיסמה שלו**

קישור זה יספק מידע על בעיות נפוצות ה יכולות להתעורר כאשר משתמש מנסה לאפס את הסיסמה שלו: בעיות [נפוצות והפתרונות שלו](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**אני נתקל בבעיה באיפוס סיסמת משתמש**

- ודא שאתה מורשה לאפס סיסמאות. *רק כללי, סיסמה ומנהלי משתמשים יכולים לאפס סיסמאות משתמש.* מנהלי מערכת כלליים יכולים גם לאפס סיסמאות של מנהל מערכת בעל הרשאות אחרות.

- ודא שאתה מבין את דרישות הרישוי:

  - לארגון שלך חייב להיות רשיון אחד לפחות:
    - **משתמשים בענן בלבד** - כל Office 365 (O365) בתשלום, או Azure AD Basic
    - **משתמשים בענן ו/או** משתמשים מקומיים - Azure AD Premium P1 או P2, Enterprise Mobility + Security (EMS) או Secure Productive Enterprise (SPE)
    - לקבלת מידע נוסף על דרישות הרישוי, ראה [דרישות רישוי](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)עבור איפוס סיסמה בשירות עצמי של Azure AD .
- כדי לאפס סיסמת משתמש, אתר את המשתמש ב- Azure AD. לאחר מכן, בלהב הסקירה עבור משתמש זה, לחץ על לחצן "איפוס סיסמה".

**לחצן איפוס הסיסמה אפור**

אינך מורשה לאפס את **הסיסמאות** של משתמש זה. *רק כללי, סיסמה ומנהלי משתמשים יכולים לאפס סיסמאות משתמש.* מנהלי מערכת כלליים יכולים גם לאפס סיסמאות של מנהל מערכת בעל הרשאות אחרות.

**איני רואה את להב איפוס הסיסמה**

אינך מורשה לאפס סיסמאות. *רק כללי, סיסמה ומנהלי משתמשים יכולים לאפס סיסמאות משתמש.* מנהלי מערכת כלליים יכולים גם לאפס סיסמאות של מנהל מערכת בעל הרשאות אחרות.

**איני רואה את להב השילוב המקומי באיפוס סיסמה**

- להב השילוב המקומי מופיע רק בסביבות היברידיות - כלומר, אתה משתמש ב- writeback באמצעות סיסמה כדי לטפל בסיסמאות של המשתמש המקומי.

- אינך רואה להב זה אם:

  - אינך משתמש בסיסמה writeback
  - ישנה בעיה בהתקנה/קישוריות של writeback של סיסמה
  - ישנה בעיה בהתקנה/קישוריות של Azure AD התחברות
  - לקבלת שלבים נוספים לפתרון בעיות בכתיבה חוזרת באמצעות סיסמה, ראה [פתרון בעיות בכתיבה חוזרת באמצעות סיסמה](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**איני יודע כיצד לאפס סיסמת משתמש**

1. היכנס לפורטל Azure כמנהל מערכת מתאים.
2. עבור אל **להב המשתמשים והקבוצות,** בחר **כל המשתמשים**.
3. בחר משתמש מהרשימה.
4. עבור המשתמש שנבחר, בחר מבט **כולל** ולאחר מכן, בשורת הפקודות, בחר **איפוס סיסמה**.
5. בחר **בלחצן איפוס** סיסמה ופעל בהתאם להוראות שעל המסך.
    - רק איפוסים שבוצעו באמצעות **Writeback של סיסמת התמיכה** בפורטל Azure.

**אני מאפס סיסמת משתמש מקומית מתוך פורטל Office 365 Admin או Office 365 למכשירים ניידים, אך המשתמש עדיין אינו יכול להיכנס**

אין תמיכה ב- Password Writeback בפורטל זה. אפס שוב את סיסמת המשתמש בפורטל Azure.
