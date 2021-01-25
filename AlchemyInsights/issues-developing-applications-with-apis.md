---
title: בעיות בפיתוח יישומים באמצעות APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974619"
---
# <a name="issues-developing-applications-with-apis"></a>בעיות בפיתוח יישומים באמצעות APIs

כדי להתחיל להשתמש ב-API של מדריכי כתובות ב-API של Active Directory, עיין [במדריך ההדרכה של הודעות מיידיות](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ב-api של תחלה, או הצג את [התיעוד האינטראקטיבי של ההפניה לשימוש](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)ב

**סיום התמיכה עבור ממשק האימות של מדריכי כתובות של Active Directory (ADAL) ו-active AD Graph API (הגרף עמ מ)**

**החל מ-30 ביוני, 2020**, לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph. אנו נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא ניתן עוד לספק עדכוני תכונות.

**החל מ-30 ביוני 2022**, נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.

יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא יקבלו שום תמיכה טכנית או עדכוני אבטחה.

יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.

**העברת ADAL**

מומלץ לעדכן את [ספריית האימות של Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה העדכניים ביותר.

אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי תאריך היעד של סיום התמיכה, ומבטיחה שיפיקו תועלת מהשיפורים המתמשכים של האבטחה והתכונות של MSAL.

1. [קרא את השאלות הנפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל היישומים שאינם של Microsoft ADAL בדייר שלך.

**העברת גרף מ-עמ**

עבור יישומים המשתמשים ב-תכלת AD Graph, בצע את ההנחיות שלנו כדי להעביר את [האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. פורטל הרישום של האפליקציה ' תכלת ' מראה אילו יישומים משתמשים ב-עמ-גרף. אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל השימוש בגרף של ה-עמ-שימוש בדייר שלך.
1. כדי שהיישום שלך ייגש לנתונים ב-Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה. [ההפניה להרשאות Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) מפרטת את ההרשאות המשויכות לכל קבוצה עיקרית של ממשקי Api של Microsoft Graph. כמו כן, הוא מספק הנחיות לגבי אופן השימוש בהרשאות.
