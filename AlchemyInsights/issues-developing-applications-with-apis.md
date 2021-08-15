---
title: בעיות בפיתוח יישומים באמצעות ממשקי API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013461"
---
# <a name="issues-developing-applications-with-apis"></a>בעיות בפיתוח יישומים באמצעות ממשקי API

כדי להתחיל להשתמש ב- API של Azure Active Directory Graph, עיין במדריך התחלה [מהירה של Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , או הצג את תיעוד ההפניה האינטראקטיבי של Azure AD Graph [API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**סיום התמיכה עבור Azure Active Directory Authentication Library (ADAL) ו- Azure AD Graph API (AAD Graph)**

**החל מ- 30 ביוני 2020,** לא נוסיף עוד תכונות חדשות לתכונות ADAL ול- Azure AD Graph. נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.

**החל מ- 30 ביוני 2022,** מסתיים התמיכה ב- ADAL וב- Azure AD Graph ולא תספק עוד תמיכה טכנית או עדכוני אבטחה.

אפליקציות המשתמשות ב- ADAL בגירסאות OS קיימות ימשיכו לפעול לאחר זמן זה, אך לא יקבלו תמיכה טכנית או עדכוני אבטחה.

אפליקציות המשתמשות ב- Azure AD Graph לאחר זמן זה עשויות שלא לקבל עוד תגובות מנקודות הקצה של Azure AD Graph נקודות הקצה.

**ADAL Migration**

אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.

אם אתה משתמש ביישומי Microsoft, תדע ש- Microsoft נמצאת בתהליך העברת היישומים שלה ל- MSAL עד למועד היעד הסופי של התמיכה, כדי להבטיח שהם ייהנו מהאבטחה השוטפת של MSAL ומהשיפורים בתכונה.

1. [קרא את שאלות נפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. אם אתה זקוק לעזרה בהבנת אילו מהאפליקציות שלך משתמשות ב- ADAL, מומלץ לסקור את כל קוד המקור של היישומים שלך, ואם ישים, ליצור קשר עם ספקי ISVS או ספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור יישומים המשתמשים ב- Azure AD Graph, בצע את ההנחיות שלנו להעברת [יישומי Azure AD Graph ל- Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת פתיחה לתחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל Graph AAD הדייר שלך.
1. כדי שהאפליקציות שלך לגשת לנתונים ב- Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה. חומר [ההפניה Graph Microsoft מפרט](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) את ההרשאות המשויכות לכל קבוצה ראשית של ממשקי API Graph Microsoft. הוא מספק גם הדרכה לגבי אופן השימוש בהרשאות.
