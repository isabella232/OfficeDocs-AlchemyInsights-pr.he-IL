---
title: פתרון בעיות כניסה יחידה (SSO) חלקה מבוססות OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745022"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>פתרון בעיות כניסה יחידה (SSO) חלקה מבוססות OIDC

- כדי ללמוד כיצד להוסיף יישום מבוסס-OIDC לדייר התכלת שלך, ראה [תחלה: הגדרת כניסה יחידה מבוססת OIDC (SSO) עבור יישום בדייר תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- לקבלת פרטים נוספים אודות אפליקציות המשתמשות בתקן החיבור של OpenID ליישום כניסה יחידה, ראה [הבנת הכניסה היחידה מבוססת על OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- לקבלת מידע למקרה שתבחר לכתוב את הקוד שלך על-ידי שליחה וטיפול ישירות בבקשות HTTP או שימוש בספריית מקור פתוחה של ספק חיצוני, במקום להשתמש באחת מספריות המקור הפתוחות שלנו, ראה [OAuth 2.0 ו-OpenID חיבור פרוטוקולים בפלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**פרוטוקולים**

1. [פלטפורמת הזהות של Microsoft וזרימת המענקים המרומזים](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) -המאפיין המגדיר של המענק המשתמע הוא שאסימונים (אסימוני מזהה או אסימוני גישה) מוחזרים ישירות מנקודת הקצה של/authorize במקום נקודת הקצה של/token. אפשרות זו משמשת לעתים קרובות כחלק מזרימת קוד ההרשאות, במה שנקרא **"flow היברידי"-אחזור אסימון המזהה בבקשת/authorize יחד עם קוד הרשאה**. מאמר זה מתאר כיצד לתכנת ישירות כנגד הפרוטוקול ביישום שלך כדי לבקש אסימונים מתכלת לספירה.
2. [זרימת קוד ההרשאות של Microsoft ו-OAuth 2.0 מתזרימה](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -ניתן להשתמש במענק קוד ההרשאות OAuth 2.0 ביישומים המותקנים במכשיר כדי לקבל גישה למשאבים מוגנים, כגון api של אינטרנט. באמצעות היישום של פלטפורמת הזהויות של Microsoft של OAuth 2.0, באפשרותך **להוסיף גישה של כניסה ו-API ליישומי הטלפון הנייד ולשולחן העבודה**. מאמר זה מתאר כיצד לתכנת ישירות כנגד הפרוטוקול ביישום שלך באמצעות כל שפה.
3. [פלטפורמת הזהות של microsoft ופרוטוקול OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -כאשר אתה משתמש ביישום הOpenID של פלטפורמת הזהויות של microsoft, באפשרותך להוסיף את הגישה של כניסה ו-API ליישומים שלך. מאמר זה מראה כיצד לעשות זאת ללא תלות בשפה ומתאר כיצד **לשלוח ולקבל הודעות HTTP מבלי להשתמש בספריות מקור פתיחה של Microsoft**.
4. [פלטפורמת הזהות של Microsoft והתזרים אישורי הלקוח של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -ניתן להשתמש במענק אישורי לקוח של OAuth 2.0 שצוין ב-RFC 6749, שנקרא לעתים **OAuth של שתי רגליים**, כדי לגשת למשאבים המתארחים באינטרנט באמצעות זהות של יישום. סוג זה של מענק משמש בדרך כלל לאינטראקציות שרת-לשרת שחייבות לפעול ברקע, ללא אינטראקציה מיידית עם משתמש. סוגי יישומים אלה מכונים לעתים קרובות **כדמון** או **כחשבונות שירות**. מאמר זה מתאר כיצד לתכנת ישירות כנגד הפרוטוקול ביישום שלך.
