---
title: בעיות באסימונים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916842"
---
# <a name="issues-with-tokens"></a>בעיות באסימונים

כדי לנהל בעיות הקשורות לאסימונים, באפשרותך לבצע את השלבים הבאים:

1. באפשרותך לציין את משך החיים של גישה, מזהה או אסימון SAML שהונפקו על-ידי פלטפורמת הזהות של Microsoft. באפשרותך להגדיר אורך חיים של אסימונים עבור כל היישומים בארגון שלך, עבור יישום רב-דייר (מרובה ארגונים), או עבור מנהל שירות ספציפי בארגון שלך. לקבלת מידע נוסף, ראה [אורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהות של Microsoft (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. אסימוני Access מאפשרים ללקוחות להתקשר באופן מאובטח לממשקי אינטרנט מוגנים, ומשתמשים ב-Api של web Api לביצוע אימות והרשאה. בהתאם למפרט OAuth, אסימונים של access הם מחרוזות אטומים ללא עיצוב מוגדר-ספקי זהויות מסוימים (IDPs) משתמשים במזהים ייחודיים, אחרים משתמשים בכתמים מוצפנים. פלטפורמת הזהויות של Microsoft משתמשת במגוון של תבניות token של access, בהתאם לקביעת התצורה של ה-API שמקבל את האסימון. כדי ללמוד כיצד ה-API שלך יכול לאמת ולהשתמש בטענות בתוך אסימון גישה, ראה [אסימוני גישה לפלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. ספריית האימות של Microsoft (MSAL) תומכת במספר זרימות אימות לשימוש בתרחישים שונים של יישומים. לקבלת מידע נוסף, ראה [זרימות אימות](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. ניתן להשתמש במענק קוד ההרשאות של OAuth 2.0 ביישומים המותקנים במכשיר כדי לקבל גישה למשאבים מוגנים, כגון רכיבי Api של אינטרנט. באמצעות היישום של פלטפורמת הזהויות של Microsoft OAuth 2.0, באפשרותך להוסיף גישה לכניסה ולממשק API ליישומי הטלפון הנייד ולשולחן העבודה. ראה את [הזרימה של קוד הזיהוי של Microsoft וזרימת קוד ההרשאות של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) לאופן התיכנות ישירות מול הפרוטוקול ביישום שלך, באמצעות כל שפה.
5. OpenID Connect (OIDC) הוא פרוטוקול אימות שנבנה ב-OAuth 2.0 שניתן להשתמש בו כדי להיכנס ליישום באופן מאובטח. כאשר אתה משתמש ביישום של נקודת הקצה של פלטפורמת הזהות של Microsoft OpenID, באפשרותך להוסיף גישת כניסה ו-API ליישומים שלך. [פלטפורמת הזהויות של microsoft ופרוטוקול החיבור של OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) מראים כיצד לעשות זאת באופן שאינו תלוי בשפה ומתארת כיצד לשלוח ולקבל הודעות HTTP ללא שימוש בספריות מקור פתיחה של microsoft.
    - נקודת הקצה של UserInfo היא חלק מ-OIDC standard, שנועד להחזיר טענות לגבי המשתמש שאומת. לקבלת מידע נוסף, ראה [נקודת קצה של פלטפורמת הזהות של UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - האפשרות [התקשרות ל-api של web app באינטרנט באמצעות המדגם ' תכלת ולOpenID](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) ' מראה כיצד לבנות יישום אינטרנט של MVC המשתמש בתכלת ad לכניסה באמצעות הפרוטוקול OpenID Connect ולאחר מכן להתקשר ל-api של אינטרנט תחת הזהות של המשתמש החתום באמצעות אסימונים שהושגו דרך OAuth 2.0. דוגמה זו משתמשת ב-OpenID חיבור ASP .Net OWIN תווכה ו-ADAL .Net.
6. [קביעת התצורה של יישום כדי לחשוף WEB api](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -בתחלה זה, עליך לרשום API של web api עם פלטפורמת הזהות של Microsoft ולחשוף אותו ליישומי לקוח על-ידי הוספת טווח דוגמה. על-ידי רישום ה-API של האינטרנט וחשיפת הטווחים, באפשרותך לספק גישה מבוססת הרשאות למשאבים שלה למשתמשים מורשים וליישומי לקוח הניגשים ל-API שלך.
7. ב-תכלת Active Directory B2C (תכלת AD B2C), הזרמת אישורי הסיסמה של בעלי המשאב (ROPC) היא זרימת אימות סטנדרטית של OAuth. בזרימה זו, יישום, הידוע גם כגורם המסתמך, מחליף אישורים חוקיים עבור אסימונים. האישורים כוללים מזהה משתמש וסיסמה. האסימונים המוחזרים הם אסימון מזהה, אסימון גישה ואסימון רענון. לקבלת מידע נוסף, ראה [הגדרת זרימת אישורים של סיסמאות של בעלי משאב בתכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

