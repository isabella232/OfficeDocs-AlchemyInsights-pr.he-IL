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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063608"
---
# <a name="issues-with-authentication-libraries"></a>בעיות בספריות אימות

1. [ספריות האימות של פלטפורמת הזהויות של microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) מפרטות את הספריות הנתמכות והתווכה של microsoft ללקוחות ולקוחות שתואמים
2. ספריית האימות של Microsoft (MSAL) תומכת במספר [זרימות אימות](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) לשימוש בתרחישים שונים של יישומים.
3. כדי לאמת ולרכוש אסימונים, עליך לאתחל יישום לקוח ציבורי או סודי חדש בקוד שלך. באפשרותך להגדיר כמה אפשרויות תצורה בעת אתחול יישום הלקוח בספריית האימות של Microsoft (MSAL). לקבלת מידע נוסף, ראה [אפשרויות תצורת יישום](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**סיום התמיכה עבור ממשק האימות של מדריכי כתובות של Active Directory (ADAL) ו-active AD Graph API (הגרף עמ מ)**

**החל מ-30 ביוני, 2020**, לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph. נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.

**החל מ-30 ביוני 2022**, נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.

יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא *יקבלו שום תמיכה טכנית או עדכוני אבטחה*.

יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.

**העברת ADAL**

אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.

אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי תאריך היעד של סיום התמיכה, ולהבטיח שייהנו מהשיפור המתמשך של האבטחה והתכונות של MSAL.

לקבלת מידע נוסף, ראה:

1. [קרא את השאלות הנפוצות בנושא ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [למד כיצד להעביר אפליקציות לפי פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור יישומים המשתמשים ב-תכלת AD Graph, בצע את ההנחיות שלנו כדי [להעביר את האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל השימוש בגרף של ה-עמ-שימוש בדייר שלך.
3. כדי שהיישום שלך ייגש לנתונים ב-Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה. [ההפניה להרשאות Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) מפרטת את ההרשאות המשויכות לכל קבוצה עיקרית של ממשקי Api של Microsoft Graph. כמו כן, הוא מספק הנחיות לגבי אופן השימוש בהרשאות.
