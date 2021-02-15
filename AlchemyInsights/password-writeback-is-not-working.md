---
title: Writeback סיסמה אינו פועל
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243366"
---
# <a name="password-writeback-is-not-working"></a>Writeback סיסמה אינו פועל

**אני נתקל בבעיות בקביעת התצורה של הסיסמה writeback**

- סיסמה writeback היא תכונה משופרת.
- ודא שהבנת את דרישות הרישוי:
  - דרוש לך רשיון אחד לפחות שהוקצה בארגון שלך
  - **משתמשים בענן בלבד** -כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic
  - **משתמשים בענן ו/או מקומיים** -תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)
    - לקבלת מידע נוסף על דרישות הרישוי, ראה [דרישות רישוי עבור איפוס סיסמה בשירות עצמי של תכלת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- יש לך לפחות חשבון מנהל אחד וחשבון משתמש אחד לבדיקה עם אחד מהרשיונות המתאימים.
- עליך לחבר את האמולטור של התכלת התחברות לאמולטור של בקר התחום הראשי עבור writeback password לעבודה. באפשרותך לקבוע את התצורה של מחבר הודעות מיידיות כדי להשתמש בבקר תחום ראשי על-ידי לחיצה ימנית על **המאפיינים** של מחבר הסינכרון של Active directory ולאחר מכן בחירה באפשרות **קבע מחיצות** משם, חפש את המקטע **הגדרות חיבור של בקר התחום** וסמן את התיבה שכותרתה **שימוש בבקרי תחום מועדפים בלבד**.
  > [!NOTE]
  > אם ה-DC המועדף אינו מהווה אמולטור של PDC, הקישור ' תכלת לספירה ' עדיין מגיע אל ה-PDC עבור writeback סיסמאות.
- איפוס הסיסמה הוגדר וזמין בדייר שלך. לקבלת מידע נוסף, ראה [הפיכת משתמשים לאיפוס סיסמאות הפרסום התכולים שלהם](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- ודא שחשבון מנהל המערכת המשמש להפיכת סיסמה Writeback הוא חשבון מנהל מערכת בענן (שנוצר באמצעות ' תכלת לספירה לא מקומית ')
- יש לך פריסה מקומית בודדת או מרובת-יערות הפועלת באמצעות פריסה מקומית של Windows Server 2008 R2, Windows Server 2012 או Windows Server 2012 R2 עם ערכות השירות העדכניות ביותר המותקנות
- הכלי ' חיבור למודע תכלת ' מותקן והכנת את סביבת הפרסום שלך לצורך סינכרון לענן. לפני שתנסה לבדוק את הסיסמה writeback, ודא שתחילה עליך להשלים את הייבוא המלא והסינכרון המלא מתוך AD ו-תכלת בחיבור של תכלת לספירה.
- לקבלת מידע נוסף, ראה כיצד לבצע [סינכרון מלא וייבוא מלא בחיבור תכלת לספירה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**אני נתקל בבעיה בקישוריות של writeback סיסמה**

1. הורד והפעל את הגירסה העדכנית ביותר של ' [תכלת לספירה](https://www.microsoft.com/download/details.aspx?id=47594) '
2. תצורת חומת אש: כלי החיבור של תכלת לספירה (1.1.443 ומעלה) יזדקק לגישת **HTTPS יוצאת** ל:
    - passwordreset.microsoftonline.com
    - servicebus. windows. נטוורקס
3. אפשר חיבורים לא פעילים להמשך לפחות 2-3 דקות

**אני עדיין נתקל בבעיות בwriteback סיסמאות**

- אם אתה עדיין נתקל בקשיים, נסה לבטל ולהפעיל מחדש את שירות writeback password בכלי ' חיבור לספירה של תכלת '
- לקבלת מידע נוסף, ראה כיצד [להפוך ללא זמין ולהפעיל מחדש את הסיסמה writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
