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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013425"
---
# <a name="issues-developing-applications"></a>בעיות בפיתוח יישומים

כדי לפתור את הבעיות הנפוצות ביותר בעת בניית אפליקציות Azure Active Directory (AD), עיין במאמרים הבאים:

- [אני רואה בעיה בכניסה ליישום באמצעות דפדפן Chrome בלבד](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [איני יודע כיצד לשנות את ברירות המחדל של משך החיים של האסימון עבור היישום שלי](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [אני מבולבל לגבי אופן העבודות של הסכמת היישום](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [איני יודע כיצד להעניק הרשאות ליישום שלי](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [איני מבין את ההבדל בין הרשאות שהוקצו להרשאות יישום](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***סיום התמיכה עבור Azure Active Directory Authentication Library (ADAL) ו- Azure AD Graph API (AAD Graph)***

- החל מ- 30 ביוני 2020, לא נוסיף עוד תכונות חדשות לספריית האימות של Azure Active Directory ‏(ADAL) ול- API של Azure AD Graph ‏(AAD Graph). נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.

- החל מ- 30 ביוני 2022 נפסיק את התמיכה עבור ADAL ו- AAD Graph ולא נספק עוד תמיכה טכנית או עדכוני אבטחה. כתוצאה מתנאים אלה, להלן ההשלכות:

    - אפליקציות המשתמשות ב- ADAL בגירסאות OS קיימות ימשיכו לפעול לאחר זמן זה, אך לא יקבלו תמיכה טכנית או עדכוני אבטחה.

    - אפליקציות המשתמשות ב Graph AAD לאחר זמן זה עשויות שלא לקבל עוד תגובות מנקודות הקצה Graph AAD

**ADAL Migration**

אם אתה משתמש באפליקציות Microsoft, מומלץ לעדכן לספריית האימות של Microsoft (MSAL), הכוללת את התכונות העדכניות ביותר ואת עדכוני האבטחה. המלצה זו נמצאת בהקשר של Microsoft המתחילה בתהליך העברת האפליקציות שלה ל- MSAL עד למועד היעד הסופי של התמיכה. 

ההעברה של Microsoft של האפליקציות שלה ל- MSAL מבטיחה שהיישומים ייהנו מהשיפורים המתמשך באבטחה ובתכונה של MSAL.

1. [קרא את השאלות הנפוצות בנושא ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [למד כיצד להעביר אפליקציות לפי פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. אם אתה זקוק לעזרה בהבנת אילו מהאפליקציות שלך משתמשות ב- ADAL, מומלץ לסקור את קוד המקור של כל היישומים שלך, ואם ישים, ליצור קשר עם ספקי תוכנה עצמאיים (ISVs) או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור יישומים המשתמשים ב- AAD Graph, בצע את ההנחיות שלנו להעברת יישומי AAD Graph ל- Microsoft Graph:

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת פתיחה לתחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. מומלץ לסקור את קוד המקור של כל היישומים שלך, ואם ישים, ליצור קשר עם ספקי תוכנה עצמאיים (ISVs) או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך מידע על השימוש Graph AAD הדייר שלך.







