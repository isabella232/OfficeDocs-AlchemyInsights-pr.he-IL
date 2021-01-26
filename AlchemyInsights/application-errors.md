---
title: שגיאות יישומים
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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984589"
---
# <a name="application-errors"></a>שגיאות יישומים

מחפש מידע לגבי **קודי השגיאה של AADSTS** המוחזרים משירות ה-"תכלת active Directory (תכלת לספירה) שירות אסימוני אבטחה (STS)? קרא את [הודעות האימות וקודי שגיאת ההרשאות](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) של ' תכלת ' כדי למצוא תיאורי שגיאות של AADSTS, תיקונים ומספר פתרונות מוצעים.

שגיאות הרשאה עשויות להיות תוצאה של כמה בעיות שונות, שרובו מייצר שגיאת 401 או 403. לדוגמה, הגורמים הבאים יכולים להוביל לשגיאות הרשאה:

- [זרימות רכישה](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) שגויות של גישת token 
- [טווחי הרשאה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) שתצורתם הוגדרה בצורה גרועה 
- חוסר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

כדי לפתור שגיאות הרשאה נפוצות, נסה את השלבים המפורטים להלן שמתאימים ביותר לשגיאה שאתה מקבל. ניתן להחיל יותר מאפשרות אחת.

**שגיאה לא מורשית של 401: האם האסימון שלך תקף?**

ודא שהיישום שלך מציג אסימון גישה חוקי ל-Microsoft Graph כחלק מהבקשה. שגיאה זו משמעותה לעתים קרובות שאסימון הגישה חסר בכותרת הבקשה לאימות HTTP או שהאסימון אינו חוקי או שפג תוקפו. אנו ממליצים מאוד להשתמש [בספריית האימות של Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) עבור רכישת אסימון גישה. בנוסף, שגיאה זו עלולה להתרחש אם אתה מנסה להשתמש באסימון גישה מוסמכות שהוענקה לחשבון Microsoft אישי כדי לגשת לממשק API התומך רק בחשבונות עבודה או בבית ספר (חשבונות ארגוניים).

**שגיאה אסורה של 403: האם בחרת את ערכת ההרשאות המתאימה?**

ודא שביקשת את ערכת ההרשאות הנכונה בהתבסס על ממשקי ה-Api של Microsoft Graph שיחות היישום שלך. הרשאות מומלצות המפורטות לפחות מוצגות בכל נושאי שיטות העזר של API של Microsoft Graph. בנוסף, יש להעניק הרשאות אלה ליישום על-ידי משתמש או מנהל מערכת. הענקת הרשאות בדרך כלל מתבצעת באמצעות דף הסכמה או על-ידי הענקת הרשאות באמצעות להב הרישום של יישום הפורטל תכלת. מתוך להב **ההגדרות** עבור היישום, לחץ על **הרשאות נדרשות** ולאחר מכן לחץ על **הענקת הרשאות**.

- [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [הכרת הרשאות מודעות של תכלת והסכמה](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**שגיאה אסורה של 403: האם האפליקציה שלך השיגה אסימון שמתאים להרשאות שבחרת?**

ודא שסוג ההרשאות ביקשו או הוענקה תואם לסוג האסימון של access שהאפליקציה רוכשת. ייתכן שאתה מבקש ומעניק הרשאות יישומים, אך משתמש באסימוני זרימת קוד אינטראקטיביים במקום באסימונים של זרימת אישורי לקוח, או מבקש ומעניק הרשאות מוסמכות אך משתמש באסימונים של זרימת אישורי לקוח במקום באסימוני זרימת קוד מוקצות.

- [קבל גישה בשם משתמשים והרשאות מוסמכות](https://docs.microsoft.com/graph/auth_v2_user) 
- [זרימת קוד ההרשאות של תכלת AD v 2.0-OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [קבל גישה ללא משתמש (שירות daemon) והרשאות יישומים](https://docs.microsoft.com/graph/auth_v2_service) 
- [זרימת אישורי לקוח של תכלת AD v 2.0-OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**שגיאה אסורה של 403: איפוס סיסמה**

בשלב זה, אין הרשאות של הרשאת שירות לשירות ב-daemon של הרשאת היישום המאפשרות איפוס סיסמאות משתמשים. ממשקי Api אלה נתמכים רק באמצעות הקוד האינטראקטיבי של הקוד המוקצה עם מנהל מערכת מחובר.

- [הרשאות Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 אסור: האם למשתמש יש גישה והוא מורשה?**

עבור זרימות קוד מועברות, Microsoft Graph מעריך אם הבקשה מותרת בהתבסס על ההרשאות שהוענקה ליישום וההרשאות שלמשתמש הנכנס יש. באופן כללי, שגיאה זו מציינת שלמשתמש אין הרשאות מספיקות כדי לבצע את הבקשה או שהמשתמש אינו מורשה לגשת לנתונים. רק משתמשים בעלי ההרשאות או הרשיונות הדרושים יכולים לבצע את הבקשה בהצלחה.

**403 אסור: האם בחרת את ה-API של משאבים נכון?**

שירותי API כגון Microsoft Graph בדוק שהתביעה האוסטרלית (קהל) באסימון הגישה שהתקבלה תואמת לערך שהוא מצפה לו, ואם לא, היא מביאה לשגיאה אסורה של 403. טעות נפוצה הנובעת משגיאה זו מנסה להשתמש באסימון שנרכש עבור ממשקי Api של הודעות מיידיות של הודעות מיידיות, Api של Outlook או SharePoint/OneDrive כדי להתקשר ל-Microsoft Graph (או להיפך). ודא שהמשאב (או הטווח) האפליקציה שלך רוכשת אסימון לצורך התאמה ל-API שאליו מתקשר היישום.

**400 בקשה שלילית או 403 אסורים: האם המשתמש מציית למדיניות הגישה המותנה (CA) של הארגון שלהם?**

בהתבסס על מדיניות של רשות אישורים של ארגון, משתמש הניגש למשאבי Microsoft Graph באמצעות האפליקציה עשוי להיות מאותגר לקבלת מידע נוסף שאינו מופיע באסימון הגישה שהאפליקציה שלך רכשה במקור. במקרה זה, האפליקציה מקבלת 400 עם שגיאת *interaction_required* במהלך רכישת אסימון של access או 403 עם שגיאת *insufficient_claims* בעת התקשרות ל-Microsoft Graph. בשני המקרים, תגובת השגיאה מכילה מידע נוסף שניתן להציג לנקודת הקצה של האישור כדי לקרוא תיגר על המשתמש לקבלת מידע נוסף (כגון אימות רב-גורמי או הרשמת מכשירים).

- [טיפול באתגרים של גישה מותנית באמצעות MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [הדרכה למפתחים עבור הגישה המותנה של תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
