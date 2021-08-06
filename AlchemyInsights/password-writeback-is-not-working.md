---
title: הסיסמה Writeback אינה פועלת
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
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999745"
---
# <a name="password-writeback-is-not-working"></a>הסיסמה Writeback אינה פועלת

**אני נתקל בבעיות בקביעת התצורה של writeback של סיסמה**

- Writeback של סיסמה הוא תכונה משופרת.
- ודא שאתה מבין את דרישות הרישוי:
  - חייב להיות לך רשיון אחד לפחות שהוקצה בארגון שלך
  - **משתמשים בענן בלבד** - כל Office 365 (O365) בתשלום, או Azure AD Basic
  - **משתמשים בענן ו/או** משתמשים מקומיים - Azure AD Premium P1 או P2, Enterprise Mobility + Security (EMS) או Secure Productive Enterprise (SPE)
    - לקבלת מידע נוסף על דרישות הרישוי, ראה [דרישות רישוי](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) עבור איפוס סיסמה בשירות עצמי של Azure AD
- יש לך חשבון מנהל מערכת אחד לפחות וחשבון מחשב משתמש אחד עם אחד מהרשיון המתאים.
- עליך לחבר את Azure AD התחברות לאמולטור בקר התחום הראשי כדי שהסיסמה writeback תעבד. באפשרותך לקבוע את התצורה של Azure AD התחברות להשתמש בבקר תחום ראשי על-ידי לחיצה באמצעות לחצן העכבר הימני על **המאפיינים** של מחבר הסינכרון של Active Directory ולאחר מכן בחירת קביעת תצורה של **מחיצות מדריך כתובות.** משם, חפש את המקטע **הגדרות החיבור של בקר** התחום ובדוק את התיבה שכותרתה השתמש **בבקרי קבוצות מחשבים מועדפת בלבד.**
  > [!NOTE]
  > אם DC המועדף אינו אמולטור PDC, Azure AD התחברות עדיין תתווסף אל ה- PDC לכתיבה חוזרת באמצעות סיסמה.
- איפוס הסיסמה הוגדר וזמין דייר שלך. לקבלת מידע נוסף, ראה [מתן אפשרות למשתמשים לאפס את סיסמאות Azure AD שלהם.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- ודא שחשבון מנהל המערכת המשמש כדי להפוך את התכונה 'כתיבת סיסמה' לזמינה היא חשבון מנהל ענן (שנוצר ב- Azure AD ולא ב- AD מקומי)
- יש לך פריסה מקומית של AD יחיד או מרובה יערות שפועלת בו Windows Server 2008 R2, Windows Server 2012 או Windows Server 2012 R2 עם ערכות ה- Service Pack העדכניות ביותר המותקנות
- התקנת את כלי התחברות Azure AD והכנת את סביבת ה- AD שלך לסינכרון לענן. לפני בדיקת הסיסמה writeback, ודא שאתה משלים תחילה ייבוא מלא וסינכרון מלא הן מ- AD וגם מ- Azure AD ב- Azure AD התחברות.
- כדי ללמוד עוד, ראה כיצד לבצע סינכרון [מלא וייבוא מלא ב- Azure AD התחברות](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**אני נתקל בבעיה בקישוריות writeback של סיסמה**

1. הורד ותפעיל את הגירסה העדכנית ביותר של [Azure AD התחברות](https://www.microsoft.com/download/details.aspx?id=47594)
2. תצורת חומת אש: הכלי Azure AD התחברות (1.1.443 ומעלה) תתצטרך גישה **יוצאת ל- HTTPS** אל:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. אפשר חיבורים לא פעילים מתמשך במשך 2-3 דקות לפחות

**אני עדיין נתקל בבעיות בכתיבה חוזרת של סיסמה**

- אם אתה עדיין נתקל בקשיים, נסה להפוך את שירות הכתיבה החוזר של הסיסמה ללא זמין התחברות Azure AD
- כדי ללמוד עוד, ראה כיצד להפוך [כתיבה חוזרת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) של סיסמה ללא זמינה וזמינה מחדש
