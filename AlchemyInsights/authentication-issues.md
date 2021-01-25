---
title: בעיות אימות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974488"
---
# <a name="authentication-issues"></a>בעיות אימות

**מחפש מידע לגבי קודי השגיאה של AADSTS המוחזרים משירות ה-"תכלת Active Directory (תכלת לספירה) שירות אסימוני אבטחה (STS)?** ראה [אימות מודעות מיידיות וקודי שגיאה של הרשאות](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) כדי למצוא תיאורי שגיאות של AADSTS, תיקונים ומספר פתרונות מוצעים.

שגיאות הרשאה עשויות להיות תוצאה של כמה בעיות שונות, שרובו מייצר שגיאת 401 או 403. לדוגמה, הבעיות הבאות יכולות להוביל לשגיאות הרשאה:

- [זרימות רכישה](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) שגויות של גישת token 
- [טווחי הרשאה](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) שתצורתם הוגדרה בצורה גרועה 
- חוסר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

כדי לפתור שגיאות הרשאה נפוצות, נסה את השלבים המפורטים להלן המתאימים ביותר לשגיאה שאתה מקבל. ניתן להחיל יותר משלב אחד עבור שגיאה שאתה מקבל.

- **שגיאה לא מורשית של 401: האם האסימון שלך תקף?**

ודא שהאפליקציה מציגה אסימון גישה חוקי ל-Microsoft Graph כחלק מהבקשה. שגיאה זו משמעותה לעתים קרובות שאסימון הגישה חסר בכותרת הבקשה לאימות HTTP או שהאסימון אינו חוקי או שפג תוקפו. אנו ממליצים מאוד להשתמש בספריית האימות של Microsoft (MSAL) עבור רכישת אסימון גישה. בנוסף, שגיאה זו עשויה להתרחש אם אתה מנסה להשתמש באסימון גישה מוסמכות שהוענקה לחשבון Microsoft אישי כדי לגשת ל-API התומך רק בחשבונות עבודה או בבית ספר (חשבונות ארגוניים).

**שגיאה אסורה של 403: האם בחרת את ערכת ההרשאות המתאימה?**

ודא שביקשת את ערכת ההרשאות הנכונה בהתבסס על ממשקי ה-Api של Microsoft Graph שיחות היישום שלך. הרשאות מומלצות עם הרשאות מומלצות מוצגות בכל נושאי שיטות העזר של API של Microsoft Graph. בנוסף, יש להעניק הרשאות אלה ליישום על-ידי משתמש או מנהל מערכת. הענקת הרשאות בדרך כלל מתבצעת באמצעות דף הסכמה או השימוש בלהב הרישום של יישום הפורטל תכלת. מתוך להב **ההגדרות** עבור היישום, לחץ על **הרשאות נדרשות** ולאחר מכן לחץ על **הענקת הרשאות**. לקבלת מידע נוסף, ראה:

- [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [הכרת הרשאות מודעות של תכלת והסכמה](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**שגיאה אסורה של 403: האם האפליקציה שלך השיגה אסימון שמתאים להרשאות שבחרת?**

ודא שסוגי ההרשאות המבוקשים או הוענקה תואמים לסוג אסימון הגישה שהאפליקציה רוכשת. ייתכן שאתה מבקש ומעניק הרשאות ליישומים, אך משתמש באסימוני זרימת קוד אינטראקטיביים במקום באסימונים של זרימת אישורי לקוח, או מבקש ומעניק הרשאות מוסמכות, אך משתמש באסימונים של זרימת האישורים של הלקוח במקום באסימונים של זרימת קוד מוקצות.

לקבלת מידע נוסף הקשור לרכישת אסימונים, ראה:

- [קבל גישה בשם משתמשים והרשאות מוסמכות](https://docs.microsoft.com/graph/auth-v2-user) 
- [זרימת קוד ההרשאות של תכלת AD v 2.0-OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [קבל גישה ללא משתמש (שירות daemon) והרשאות יישומים](https://docs.microsoft.com/graph/auth-v2-service) 
- [זרימת אישורי לקוח של תכלת AD v 2.0-OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**שגיאה אסורה של 403: איפוס סיסמה**

בשלב זה, אין הרשאות של הרשאת שירות לשירות ב-daemon של הרשאת היישום המאפשרות איפוס סיסמאות משתמשים. ממשקי Api אלה נתמכים רק באמצעות הקוד האינטראקטיבי של הקוד המוקצה עם מנהל מערכת מחובר. לקבלת מידע נוסף, ראה [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 אסור: האם למשתמש יש גישה והוא מורשה?**

עבור זרמי קוד מוסמכים, Microsoft Graph מעריך אם הבקשה הועברה בהתבסס על ההרשאות שהתקבלו ליישום וההרשאות שלמשתמש הנכנס יש. באופן כללי, שגיאה זו מציינת שלמשתמש אין הרשאות מספיקות כדי לבצע את הבקשה **או** שהמשתמש אינו מורשה לגשת לנתונים. רק משתמשים בעלי ההרשאות או הרשיונות הדרושים יכולים לבצע את הבקשה בהצלחה.

**403 אסור: האם בחרת את ה-API של משאבים נכון?**

API services כגון Microsoft Graph ודא שהתביעה *האוסטרלית* (קהל) באסימון הגישה שהתקבלה תואמת לערך שהוא מצפה לו, ואם לא, תתרחש שגיאה אסורה של 403. טעות נפוצה הנובעת משגיאה זו מנסה להשתמש באסימון שנרכש עבור ממשקי Api של הודעות מיידיות של הודעות מיידיות, Api של Outlook או SharePoint/OneDrive כדי להתקשר ל-Microsoft Graph (או להיפך). ודא שהמשאב (או הטווח) האפליקציה שלך רוכשת אסימון לצורך התאמה ל-API שאליו מתקשר היישום.

**400 בקשה שלילית או 403 אסורים: האם המשתמש מציית למדיניות הגישה המותנה (CA) של הארגון שלהם?**

בהתבסס על מדיניות גישה מותנית של ארגון (CA), משתמש הניגש למשאבי Microsoft Graph באמצעות האפליקציה שלך עשוי להיות מאותגר לקבלת מידע נוסף שאינו מופיע באסימון הגישה שהאפליקציה שלך רכשה במקור. במקרה זה, האפליקציה מקבלת **400 עם שגיאת *interaction_required*** במהלך רכישת אסימון של access או **403 עם שגיאת *insufficient_claims*** בעת התקשרות ל-Microsoft Graph. בשני המקרים, תגובת השגיאה מכילה מידע נוסף שניתן להציג לנקודת הקצה המורשה כדי לאתגר את המשתמש לקבלת מידע נוסף (כגון אימות רב-גורמי או הרשמת מכשירים).

לקבלת מידע נוסף הקשור לגישה מותנית, ראה:

- [טיפול באתגרים של גישה מותנית באמצעות MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [הדרכה למפתחים עבור הגישה המותנה של תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_סיום התמיכה עבור כללי האימות של מדריכי הכתובות של Active Directory (ADAL) וממשק תכלת של הודעות מיידיות ב-API (הגרף עמ מ)_* _

- החל מ-30 ביוני, 2020, לא נוסיף עוד תכונות חדשות לספריית האימות של Active Directory (ADAL) והתכלת הגרפי של הודעות מיידיות (API). אנו נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא ניתן עוד לספק עדכוני תכונות.
- החל מ-30 ביוני 2022, אנו נסיים את התמיכה עבור ADAL ו-עמ-עמ והוא לא יספק עוד תמיכה טכנית או עדכוני אבטחה.
    - יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא יקבלו שום תמיכה טכנית או עדכוני אבטחה.
    - אפליקציות המשתמשות בגרף של ה-עמ לאחר שעה זו עשויות לקבל תגובות מנקודת הקצה של גרף ה-עמ.

_ *העברה של ADAL**

מומלץ לעדכן את [ספריית האימות של Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה העדכניים ביותר. המלצה זו ממוקמת בהקשר של Microsoft מעבירה את היישומים שלה ל-MSAL על-ידי מועד היעד של סוף התמיכה. המטרה של העברת האפליקציות של Microsoft ל-MSAL היא להבטיח שהיישומים ירוויחו מהאבטחה המתמשכת של MSAL ושיפורים בתכונות.

- [קריאת השאלות הנפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי תוכנה עצמאיים (Isv) או לספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל היישומים שאינם של Microsoft ADAL בדייר שלך.

**העברת גרף מ-עמ**

עבור יישומים המשתמשים בגרף של ה-עמ, בצע את ההנחיות שלנו כדי [להעביר את האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- פורטל הרישום של האפליקציה ' תכלת ' מראה אילו יישומים משתמשים ב-עמ-גרף. אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים. התמיכה של Microsoft יכולה גם לספק לך את המידע של כל השימוש בגרף של ה-עמ בדייר שלך.

 










