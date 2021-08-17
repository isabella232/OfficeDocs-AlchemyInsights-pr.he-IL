---
title: פתרון בעיות כניסה יחידה (SSO) מבוססות OIDC
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105779"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>פתרון בעיות כניסה יחידה (SSO) מבוססות OIDC

- כדי ללמוד כיצד להוסיף יישום מבוסס OIDC לדייר Azure שלך, ראה התחלה מהירה: הגדרת כניסה יחידה [מבוססת OIDC (SSO) עבור](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)יישום הדייר של Azure Active Directory (Azure AD).
- לקבלת פרטים נוספים אודות אפליקציות המשתמשות בתקן OpenID התחברות ליישם כניסה יחידה, ראה הבנת כניסה יחידה [מבוססת OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- לקבלת מידע במקרה שתבחר לכתוב את הקוד שלך על-ידי שליחה וטיפול ישירות בבקשות HTTP או שימוש בספריית קוד פתוח של ספקים חיצוניים, במקום להשתמש באחת מספריות הקוד הפתוח שלנו, ראה [OAuth 2.0 ופרוטוקולי OpenID התחברות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)ב- פלטפורמת הזהויות של Microsoft.

**פרוטוקולים**

1. [פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) ומענק זרימה מפורש - המאפיין המעניק המשתתפי הוא שאסימונים (אסימוני מזהה או אסימוני גישה) מוחזרים ישירות מתוך נקודת הקצה /authorize במקום נקודת הקצה /token. פעולה זו משמשת לעתים קרובות כחלק מזרימת קוד ההרשאה, במה שנקרא "זרימה היברידית" - אחזור אסימון המזהה בבקשה **/authorize יחד עם קוד הרשאה.** מאמר זה מתאר כיצד לתכנת ישירות מול הפרוטוקול ביישום שלך כדי לבקש אסימונים מ- Azure AD.
2. פלטפורמת הזהויות של Microsoft וזרימת קוד [הרשאה של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - ניתן להשתמש במענק קוד ההרשאות של OAuth 2.0 באפליקציות המותקנות במכשיר כדי לקבל גישה למשאבים מוגנים, כגון ממשקי API באינטרנט. באמצעות פלטפורמת הזהויות של Microsoft של OAuth 2.0, באפשרותך להוסיף גישת כניסה ו- **API לאפליקציות הניידות ולאפליקציות שולחן העבודה שלך.** מאמר זה מתאר כיצד לתכנת ישירות מול הפרוטוקול ביישום שלך באמצעות שפה כלשהי.
3. [פלטפורמת הזהויות של Microsoft ופרוטוקול OpenID התחברות](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - בעת שימוש ביישום OpenID פלטפורמת הזהויות של Microsoft של התחברות, באפשרותך להוסיף גישת כניסה ו- API ליישומים שלך. מאמר זה מראה כיצד לעשות זאת ללא קשר לשפה ומתאר כיצד לשלוח **ולקבל הודעות HTTP מבלי להשתמש בספריות קוד פתוח של Microsoft.**
4. פלטפורמת הזהויות של Microsoft וזרימת אישורי לקוח [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - באפשרותך להשתמש במענק אישורי הלקוח OAuth 2.0 שצוינו ב- RFC 6749, הנקרא לעתים **OAuth דו-רגליים**, כדי לגשת למשאבים המתארחים באינטרנט באמצעות זהות יישום. מענק מסוג זה משמש בדרך כלל עבור אינטראקציות בשרת לשרת שיש לפעול ברקע, ללא אינטראקציה מיידית עם משתמש. סוגים אלה של יישומים נקראים לעתים קרובות **Daemons או** **חשבונות שירות**. מאמר זה מתאר כיצד לתכנת ישירות מול הפרוטוקול ביישום שלך.
