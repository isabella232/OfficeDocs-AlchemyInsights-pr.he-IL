---
title: שגיאות יישום
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
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931450"
---
# <a name="application-errors"></a>שגיאות יישום

מחפש מידע אודות קודי **השגיאה של AADSTS** המוחזרים משירות אסימון האבטחה (STS) של Azure Active Directory (Azure AD)? קרא [קודי שגיאה של אימות והרשאות של Azure AD כדי](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) למצוא תיאורי שגיאות של AADSTS, תיקונים וחלק מהפתרונות המוצעים לעקיפת הבעיה.

שגיאות הרשאה יכולות להיגרם ממספר בעיות שונות, כאשר רובן מייצרות את השגיאות 401 או 403. לדוגמה, כל הפעולות הבאות יכולות להוביל לשגיאות מתן הרשאות:

- [זרימות רכישה שגויות של אסימוני גישה](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [טווחי הרשאות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) שתצורתם לא נקבעה כהלכה 
- היעדר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

כדי לפתור שגיאות הרשאה נפוצות, נסה את השלבים המפורטים להלן התואמים ביותר לשגיאה שאתה מקבל. יותר מפעם אחת עשויים לחול.

**שגיאת 'לא מורשה' 401: האם האסימון שלך חוקי?**

ודא שהיישום שלך מציג אסימון גישה חוקי ל- Microsoft Graph כחלק מהבקשה. לעיתים קרובות פירוש שגיאה זו הוא שבכותרת בקשת האימות של HTTP אסימון הגישה חסר, או שהאסימון אינו חוקי או שתוקפו פג. מומלץ מאוד להשתמש בספריית האימות [של Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) לרכישת אסימון גישה. בנוסף, שגיאה זו עשויה להתרחש אם אתה מנסה להשתמש באסימון גישה מוסמך המוענק לחשבון Microsoft אישי כדי לגשת ל- API התומך רק בחשבונות בעבודה או בבית ספר (חשבונות ארגוניים).

**שגיאת 'אסור' 403: האם בחרת את ערכת ההרשאות הנכונה?**

ודא שביקשת את ערכת ההרשאות הנכונה בהתבסס על ממשקי ה- API של Microsoft Graph היישומים שלך. הרשאות מומלצות הפחות הרשאות מסופקות בכל נושאי שיטת ההפניה של Microsoft Graph API. בנוסף, הרשאות אלה חייבות להיות מוענקות לאפליקציה על-ידי משתמש או מנהל מערכת. הענקת הרשאות מתרחשת בדרך כלל דרך דף הסכמה או על-ידי הענקת הרשאות באמצעות להב הרישום של יישום Azure Portal. מתוך ה- Blade **הגדרות** עבור האפליקציה, לחץ על **ההרשאות הנדרשות** ולאחר מכן לחץ על **הענק הרשאות**.

- [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [הבנת ההרשאות וההסכמה של Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**שגיאת 'אסור' 403: האם האפליקציה שלך רכשה אסימון מתאים להרשאות שנבחרו?**

ודא שסוג ההרשאות המבוקש או שהוענק תואם לסוג אסימון הגישה שהיישום שלך רוכש. ייתכן שאתה מבקש ומעניק הרשאות יישום אך משתמש באסימוני זרימת קוד אינטראקטיביים שהוקצו במקום באסימוני זרימת אישור של לקוח, או מבקש ומעניק הרשאות שהוקצו, אך משתמש באסימוני זרימת אישור של לקוח במקום באסימוני זרימת קוד שהוקצו.

- [קבלת גישה בשם המשתמשים והרשאות מוקצות](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - זרימת קוד הרשאה של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [קבלת גישה ללא משתמש (שירות Daemon) והרשאות אפליקציה](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - זרימת אישורי לקוח של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**שגיאת 'אסור' 403: איפוס סיסמה**

בשלב זה, אין הרשאות שירות-לשירות של Daemon של הרשאות אפליקציה המאפשרות איפוס סיסמאות משתמשים. ממשקי API אלה נתמכים רק באמצעות זרימות קוד אינטראקטיבי מוקצות עם מנהל מערכת מחובר.

- [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 'אסור': האם למשתמש יש גישה והאם יש לו רשיון?**

עבור זרימה של קוד Graph, Microsoft Graph אם הבקשה מותרת בהתבסס על ההרשאות שהוענקו לאפליקציה וההרשאות שיש למשתמש הכניסה. באופן כללי, שגיאה זו מציינת כי למשתמש אין הרשאות מספיקות כדי לבצע את הבקשה או שלמשתמש אין רשיון לגישה לנתונים. רק משתמשים בעלי ההרשאות או הרשיונות הדרושים יכולים לבצע את הבקשה בהצלחה.

**403 'אסור': האם בחרת את ה- API של המשאב הנכון?**

שירותי API כמו Microsoft Graph לבדוק שטענת השידור (קהל) באסימון הגישה שהתקבלה תואמת לערך שהוא מצפה לו, ואם לא, היא תקבל שגיאה אסורה 403. טעות נפוצה שגורמת לשגיאה זו היא הניסיון להשתמש באסימון שנרכש עבור ממשקי API של Azure AD Graph, ממשקי API של Outlook או ממשקי API של SharePoint/OneDrive כדי לקרוא ל- Microsoft Graph (או להפך). ודא כי המשאב (או הטווח) שהאפליקציה שלך רוכשת אסימון עבורו תואם ל- API שהאפליקציה קוראת לו.

**400 'בקשה שגויה' או '403 אסור': האם המשתמש מציית לפריטי מדיניות הגישה המותנה (CA) של הארגון שלו?**

בהתבסס על מדיניות רשות אישורים של ארגון, ייתכן שמשתמש ניגש למשאבי Microsoft Graph דרך האפליקציה שלך לקבלת מידע נוסף שלא נמצא באסימון הגישה שבו האפליקציה רכשה במקור. במקרה זה, האפליקציה שלך תקבל שגיאת 400 עם *interaction_required* במהלך רכישת אסימון הגישה או שגיאת 403 עם *insufficient_claims* בעת קריאה ל- Microsoft Graph. בשני המקרים, תגובת השגיאה מכילה מידע נוסף ש ניתן להציג לנקודות הקצה המאשרות לאתגר את המשתמש לקבלת מידע נוסף (כמו אימות רב-גורמי או הרשמה למכשירים).

- [טיפול באתגרי גישה מותנים באמצעות MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [הדרכה למפתחים בנושא גישה מותנית ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
