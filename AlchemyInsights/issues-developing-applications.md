---
title: בעיות בפיתוח יישומים
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
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974474"
---
# <a name="issues-developing-applications"></a>בעיות בפיתוח יישומים

כדי לפתור את הבעיות הנפוצות ביותר בעת בניית יישומי תכלת של Active Directory (AD), עיין במאמרים הבאים:

- [אני רואה בעיות כניסה ליישומים באמצעות דפדפן Chrome בלבד](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [איני יודע כיצד לשנות את ברירות המחדל של כל החיים של האסימון עבור היישום שלי](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [אני מבולבל לגבי אופן הפעולה של הסכמת היישום](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [איני יודע כיצד להעניק הרשאות ליישום שלי](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [איני מבין את ההבדל בין הרשאות מוקצות והרשאות יישום](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***סיום התמיכה עבור כללי האימות של מדריכי הכתובות של Active Directory (ADAL) וממשק תכלת של הודעות מיידיות ב-API (הגרף עמ מ)** _

- החל מ-30 ביוני, 2020, לא נוסיף עוד תכונות חדשות לספריית האימות של Active Directory (ADAL) והתכלת הגרפי של הודעות מיידיות (API). אנו נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא ניתן עוד לספק עדכוני תכונות.

- החל מ-30 ביוני 2022, אנו נסיים את התמיכה עבור ADAL ו-עמ-עמ והוא לא יספק עוד תמיכה טכנית או עדכוני אבטחה. כתוצאה מתנאי זה, להלן ההשלכות:

    - יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא יקבלו שום תמיכה טכנית או עדכוני אבטחה.

    - יישומים באמצעות גרף עמ-משתמשים לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של גרף ה-עמ

_ *העברה של ADAL**

אם אתה משתמש ב-Microsoft apps, מומלץ לעדכן לספריית האימות של Microsoft (MSAL), הכוללת את התכונות ועדכוני האבטחה העדכניים ביותר. המלצה זו נמצאת בהקשר של Microsoft היוזמת את תהליך העברת האפליקציות שלה ל-MSAL על-ידי מועד היעד של סוף התמיכה. 

ההעברה על-ידי Microsoft של היישומים שלה ל-MSAL מבטיחה שהיישומים ירוויחו מהאבטחה המתמשכת של MSAL ושיפורים בתכונות.

1. [קריאת השאלות הנפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים שלך, ובמידת הצורך, להושיט יד לכל ספקי תוכנה עצמאיים (Isv) או לספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל היישומים שאינם של Microsoft ADAL בדייר שלך.

**העברת גרף מ-עמ**

עבור יישומים המשתמשים בגרף של ה-עמ, פעל לפי ההנחיות שלנו כדי להעביר את האפליקציות של גרף עמ ' ל-Microsoft Graph:

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. פורטל הרישום של האפליקציה ' תכלת ' מראה אילו יישומים משתמשים ב-עמ-גרף. אנו ממליצים לך לסקור את כל קוד המקור של היישומים שלך, ובמידת הצורך, להושיט יד לכל ספקי תוכנה עצמאיים (Isv) או לספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך מידע אודות השימוש בגרף של שימוש בגרף של הדייר.







