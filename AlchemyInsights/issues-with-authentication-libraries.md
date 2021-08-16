---
title: בעיות בספריות אימות
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028005"
---
# <a name="issues-with-authentication-libraries"></a>בעיות בספריות אימות

1. [פלטפורמת הזהויות של Microsoft אימות מפורטות](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) ספריות לקוח ותוכנות ביניים הנתמכות על-ידי Microsoft ותואמות.
2. ספריית האימות של Microsoft (MSAL) תומכת [במספר זרימות אימות](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) לשימוש בתרחישי יישומים שונים.
3. כדי לאמת ולהשיג אסימונים, עליך לאתחל יישום לקוח ציבורי או סודי חדש בקוד שלך. באפשרותך להגדיר כמה אפשרויות תצורה בעת אתחול יישום הלקוח בספריית האימות של Microsoft (MSAL). כדי ללמוד עוד, ראה [אפשרויות תצורת יישום](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**סיום התמיכה עבור Azure Active Directory Authentication Library (ADAL) ו- Azure AD Graph API (AAD Graph)**

**החל מ- 30 ביוני 2020,** לא נוסיף עוד תכונות חדשות לתכונות ADAL ול- Azure AD Graph. נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.

**החל מ- 30 ביוני 2022,** מסתיים התמיכה ב- ADAL וב- Azure AD Graph ולא תספק עוד תמיכה טכנית או עדכוני אבטחה.

אפליקציות המשתמשות ב- ADAL בגירסאות OS קיימות ימשיכו לפעול לאחר זמן זה, אך לא יתעדכו תמיכה *טכנית או עדכוני אבטחה.*

אפליקציות המשתמשות ב- Azure AD Graph לאחר זמן זה עשויות שלא לקבל עוד תגובות מנקודות הקצה של Azure AD Graph נקודות הקצה.

**ADAL Migration**

אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.

אם אתה משתמש ביישומי Microsoft, תדע ש- Microsoft נמצאת בתהליך העברת היישומים שלה ל- MSAL עד למועד היעד הסופי של התמיכה, כדי להבטיח שהם ייהנו מהשיפורים המתמשך באבטחה ובתכונה של MSAL.

לקבלת מידע נוסף, ראה:

1. [קרא את השאלות הנפוצות בנושא ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [למד כיצד להעביר אפליקציות לפי פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. אם אתה זקוק לעזרה בהבנת אילו מהאפליקציות שלך משתמשות ב- ADAL, מומלץ לסקור את כל קוד המקור של היישומים שלך, ואם ישים, ליצור קשר עם ספקי ISVS או ספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור יישומים המשתמשים ב- Azure AD Graph, בצע את ההנחיות שלנו להעברת [יישומי Azure AD Graph ל- Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [רשימת הפעולות לביצוע של ההעברה שלנו מספקת נקודת תחילת העבודה.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל Graph AAD הדייר שלך.
3. כדי שהאפליקציות שלך לגשת לנתונים ב- Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה. חומר [ההפניה Graph Microsoft מפרט](https://docs.microsoft.com/graph/permissions-reference) את ההרשאות המשויכות לכל קבוצה ראשית של ממשקי API Graph Microsoft. הוא מספק גם הדרכה לגבי אופן השימוש בהרשאות.
