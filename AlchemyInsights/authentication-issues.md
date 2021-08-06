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
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019509"
---
# <a name="authentication-issues"></a>בעיות אימות

**מחפש מידע על קודי שגיאות של AADSTS המוחזרים משירות אסימוני האבטחה (STS) של Azure Active Directory‏ (Azure AD)?** ראה [קודי שגיאה של אימות והרשאה ב- Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) כדי למצוא תיאורי שגיאות של AADSTS, תיקונים ומספר פתרונות מוצעים.

שגיאות הרשאה יכולות להיגרם ממספר בעיות שונות, כאשר רובן מייצרות את השגיאות 401 או 403. לדוגמה, כל הבעיות הבאות עלולות להוביל לשגיאות הרשאה:

- [זרימות רכישה שגויות של אסימוני גישה](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- [טווחי הרשאות](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) שתצורתם לא נקבעה כהלכה 
- היעדר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

כדי לפתור שגיאות הרשאה נפוצות, נסה לבצע את אלו מבין השלבים המפורטים להלן אשר מתאימים במידה הרבה ביותר לשגיאה שאתה מקבל. ייתכן שיותר משלב אחד יתאים לשגיאה שאתה מקבל.

**שגיאת 'לא מורשה' 401: האם האסימון שלך חוקי?**

ודא שהאפליקציה שלך מציגה אסימון גישה חוקי ל- Microsoft Graph כחלק מהבקשה. לעיתים קרובות פירוש שגיאה זו הוא שבכותרת בקשת האימות של HTTP אסימון הגישה חסר, או שהאסימון אינו חוקי או שתוקפו פג. אנו ממליצים להשתמש בספריית האימות של Microsoft (MSAL) לרכישת אסימון גישה. בנוסף, שגיאה זו עשויה להתרחש אם אתה מנסה להשתמש באסימון גישה מוקצה שהוענק לחשבון Microsoft אישי כדי לגשת ל- API התומך רק בחשבונות בעבודה או בבית ספר (חשבונות ארגוניים).

**שגיאת 'אסור' 403: האם בחרת את ערכת ההרשאות הנכונה?**

ודא שביקשת את ערכת ההרשאות הנכונה בהתבסס על ממשקי ה- API של Microsoft Graph עבור קריאות האפליקציה שלך. ההרשאות המינימליות המומלצות מצוינות בכל נושאי התיעוד של מתודות ה- API של Microsoft Graph. בנוסף, הרשאות אלה חייבות להיות מוענקות לאפליקציה על-ידי משתמש או מנהל מערכת. הענקת הרשאות מתרחשת בדרך כלל באמצעות דף הסכמה או שימוש ב- Blade של רישום האפליקציות בפורטל Azure. מתוך ה- Blade **הגדרות** עבור האפליקציה, לחץ על **ההרשאות הנדרשות** ולאחר מכן לחץ על **הענק הרשאות**. לקבלת מידע נוסף, ראה:

- [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [הבנת ההרשאות וההסכמה של Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**שגיאת 'אסור' 403: האם האפליקציה שלך רכשה אסימון מתאים להרשאות שנבחרו?**

ודא כי סוגי ההרשאות שהתבקשו או שהוענקו מתאימים לסוג אסימון הגישה שהאפליקציה שלך רוכשת. ייתכן שאתה מבקש ומעניק הרשאות אפליקציה, אך משתמש באסימוני זרימת קוד אינטראקטיבי מוקצים במקום באסימוני זרימה של אישורי לקוח, או מבקש ומעניק הרשאות מוקצות אך משתמש באסימוני זרימה של אישורי לקוח במקום באסימוני זרימת קוד מוקצים.

לקבלת מידע נוסף הקשור לרכישת אסימונים, ראה:

- [קבלת גישה בשם המשתמשים והרשאות מוקצות](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - זרימת קוד הרשאה של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [קבלת גישה ללא משתמש (שירות Daemon) והרשאות אפליקציה](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - זרימת אישורי לקוח של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**שגיאת 'אסור' 403: איפוס סיסמה**

בשלב זה, אין הרשאות שירות-לשירות של Daemon של הרשאות אפליקציה המאפשרות איפוס סיסמאות משתמשים. ממשקי API אלה נתמכים רק באמצעות זרימות קוד אינטראקטיבי מוקצות עם מנהל מערכת מחובר. לקבלת מידע נוסף, ראה [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 'אסור': האם למשתמש יש גישה והאם יש לו רשיון?**

עבור זרימות קוד מוקצות, Microsoft Graph בודק אם ניתן אישור לבקשה בהתבסס על ההרשאות שהוענקו לאפליקציה ולהרשאות שבהן מחזיק המשתמש המחובר. באופן כללי, שגיאה זו מציינת כי למשתמש אין הרשאות מספיקות כדי לבצע את הבקשה **או** שלמשתמש אין רשיון לגישה לנתונים. רק משתמשים בעלי ההרשאות או הרשיונות הדרושים יכולים לבצע את הבקשה בהצלחה.

**403 'אסור': האם בחרת את ה- API של המשאב הנכון?**

שירותי API כגון Microsoft Graph בודקים שבקשת ה *aud* (קהל) באסימון הגישה שהתקבל תואמת לערך שהם מצפים לו, ואם לא, מתרחשת שגיאת 403 'אסור'. טעות נפוצה שגורמת לשגיאה זו היא הניסיון להשתמש באסימון שנרכש עבור ממשקי API של Azure AD Graph, ממשקי API של Outlook או ממשקי API של SharePoint/OneDrive כדי לקרוא ל- Microsoft Graph (או להפך). ודא כי המשאב (או הטווח) שהאפליקציה שלך רוכשת אסימון עבורו תואם ל- API שהאפליקציה קוראת לו.

**400 'בקשה שגויה' או '403 אסור': האם המשתמש מציית לפריטי מדיניות הגישה המותנה (CA) של הארגון שלו?**

בהתבסס על מדיניות הגישה המותנה (CA) של הארגון, ייתכן שמשתמש שניגש למשאבים של Microsoft Graph דרך האפליקציה שלך יידרש לספק מידע נוסף שאינו נמצא באסימון הגישה שהאפליקציה שלך רכשה במקור. במקרה זה, האפליקציה שלך תקבל שגיאת **400 עם *interaction_required*** במהלך רכישת אסימון הגישה או שגיאת **403 עם *insufficient_claims*** בעת קריאה ל- Microsoft Graph. בשני המקרים, תגובת השגיאה מכילה מידע נוסף שניתן להציג בנקודת הקצה המורשית כדי לבקש מהמשתמש לספק מידע נוסף (כמו אימות רב-גורמי או רישום מכשירים).

לקבלת מידע נוסף בנוגע לגישה מותנית, ראה:

- [טיפול באתגרי גישה מותנית באמצעות MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [הדרכה למפתחים בנושא גישה מותנית ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***סיום התמיכה עבור Azure Active Directory Authentication Library (ADAL) ו- Azure AD Graph API (AAD Graph)***

- החל מ- 30 ביוני 2020, לא נוסיף עוד תכונות חדשות לספריית האימות של Azure Active Directory ‏(ADAL) ול- API של Azure AD Graph ‏(AAD Graph). נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.
- החל מ- 30 ביוני 2022 נפסיק את התמיכה עבור ADAL ו- AAD Graph ולא נספק עוד תמיכה טכנית או עדכוני אבטחה.
    - אפליקציות המשתמשות ב- ADAL בגירסאות OS קיימות ימשיכו לפעול לאחר זמן זה, אך לא יקבלו תמיכה טכנית או עדכוני אבטחה.
    - אפליקציות שישתמשו ב- AAD Graph לאחר מועד זה עלולות לא לקבל עוד תגובות מנקודת הקצה של AAD Graph.

**ADAL Migration**

אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים. המלצה זו ניתנת לאור העובדה ש- Microsoft תעביר את האפליקציות שלה ל- MSAL לפני תאריך היעד של סיום התמיכה. מטרת ההעברה של אפליקציות Microsoft ל- MSAL היא להבטיח שהאפליקציות יפיקו תועלת מהשיפורים המתמשכים באבטחה ובתכונות של MSAL.

- [קרא את השאלות הנפוצות בנושא ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [למד כיצד להעביר אפליקציות לפי פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- אם אתה זקוק לעזרה כדי להבין אילו מהאפליקציות שלך משתמשות ב- ADAL, מומלץ לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ספקי תוכנה עצמאיים (ISVs) או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור אפליקציות המשתמשות ב- AAD Graph, בצע את ההנחיות שלנו [להעברת אפליקציות של Azure AD Graph ל- Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [רשימת הפעולות לביצוע של ההעברה מספקת נקודת פתיחה לתחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך מידע על כל השימוש ב- AAD Graph בדייר שלך.

 










