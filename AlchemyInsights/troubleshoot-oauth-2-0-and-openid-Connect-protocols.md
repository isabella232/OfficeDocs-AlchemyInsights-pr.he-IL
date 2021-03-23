---
title: פתרון בעיות בפרוטוקולים OAuth 2.0 ו-OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036407"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>פתרון בעיות בפרוטוקולים OAuth 2.0 ו-OpenID Connect

כדי לפתור את בעיות החיבור של OAuth 2.0 ו-OpenID, בצע את השלבים המומלצים הבאים:

עיין במאמרים הבאים הקשורים לתצורה ולפתרון בעיות בפרוטוקולים OAuth 2.0 ו-OpenID Connect:

- מאמר זה מתאר את [הזרימה של פלטפורמת הזהות של Microsoft ואת OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -מאמר זה מתאר כיצד לתכנת ישירות נגד **הזרימה של מענק הקוד (PKCE)** ביישום שלך, באמצעות כל שפה.
- [פלטפורמת הזהויות של Microsoft וזרימת אישורי הלקוח של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -מאמר זה מתאר כיצד לתכנת ישירות כנגד **זרימת אישורי הלקוח** ביישום שלך.
- מאמר זה מתאר כיצד לתכנת ישירות לגבי **הזרימה של ROPC** ביישום שלך [באמצעות Microsoft identity Platform platform 2.0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) .
    - פלטפורמת הזהויות של Microsoft תומכת רק ב-ROPC עבור דיירים של הודעות מיידיות, ולא עבור חשבונות אישיים. משמעות הדבר היא שעליך להשתמש בנקודת קצה ספציפית לדייר **https://login.microsoftonline.com/{TenantId_or_Name}) (** או בנקודת הקצה של **הארגונים** .
    - חשבונות אישיים המוזמנים לדייר המודע של תכלת אינם יכולים להשתמש ב-ROPC.
    - חשבונות שאין להם סיסמאות אינם מצליחים להיכנס דרך ROPC. בתרחיש זה, מומלץ להשתמש בזרימה אחרת עבור האפליקציה שלך, במקום זאת.
    - אם המשתמשים צריכים להשתמש [באימות רב-גורמי (מנהל מכשפות)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) כדי להיכנס ליישום, הם ייחסמו.
    - ROPC אינו נתמך בתרחישים של [האיחוד הזהויות ההיברידית](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (לדוגמה, התכלת המודע ו-ADFS המשמשים לאימות חשבונות מקומיים). אם משתמשים בעלי עמוד מלא מנותבים מחדש לספק זהויות מקומי, לתכלת לספירה אין אפשרות לבדוק את שם המשתמש והסיסמה כנגד ספק הזהויות. [אימות מעבר](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) נתמך עם ROPC, עם זאת.
    - חריגה לתרחיש האיחוד של זהויות היברידיות תהיה הדוגמה הבאה: מדיניות גילוי תחום הבית עם **AllowCloudPasswordValidation** מוגדר ל- **TRUE** תאפשר זרימה של ROPC כדי לעבוד עבור משתמשים מאוחדים כאשר סיסמה מקומית מסונכרנת לענן. לקבלת מידע נוסף, ראה [הפיכת אימות ROPC ישיר של משתמשים מאוחדים לזמינים עבור יישומים מדור קודם](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [פלטפורמת הזהות של Microsoft ו-OAuth 2.0 מטעם הזרימה-מאמר](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) זה מתאר כיצד לתכנת ישירות מול הזרימה המדוברת **של (OBO)** ביישום שלך.
- [פלטפורמת הזהות של Microsoft ופרוטוקול החיבור של OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -מאמר זה מראה כיצד ליישם את פרוטוקול החיבור של OpenID ללא שימוש בשפה, ומתאר כיצד לשלוח ולקבל הודעות HTTP מבלי להשתמש בספריות מקור Open של microsoft.

**אסימוני גישה**

[אסימוני גישה לפלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -למד כיצד ה-API שלך יכול לאמת ולהשתמש בטענות בתוך אסימון גישה. כל התיעוד במאמר זה, למעט היכן שצוין, חל רק על אסימונים שהונפקו עבור APIs שנרשמת. הוא אינו חל על אסימונים שהונפקו עבור ממשקי Api בבעלות Microsoft, וגם לא ניתן להשתמש באסימונים אלה כדי לאמת את האופן שבו פלטפורמת הזהות של Microsoft תיצור אסימונים עבור ממשק API שאתה יוצר.

**תצורת יישום**

[ניתוב מחדש של uri (כתובת url של השב) ומגבלות](https://docs.microsoft.com/azure/active-directory/develop/reply-url) -למד כיצד לקבוע את התצורה של uri הניתוב מחדש (כתובת url של השב). כתובת URL של ' ניתוב מחדש ' או ' השב ', היא המיקום שבו שרת ההרשאות שולח את המשתמש לאחר שהיישום הוסמך בהצלחה ומקבל קוד הרשאה או אסימון גישה. שרת ההרשאות שולח את הקוד או האסימון לאורי הניתוב מחדש; לכן חשוב לרשום את המיקום הנכון כחלק מתהליך הרישום של האפליקציה.

**הקצאת יישומים**

[ערכת לימוד: פיתוח ותכנון הקצאת משאבים עבור נקודת קצה של SCIM-מאמר](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) זה מתאר כיצד לבנות נקודת קצה של SCIM ולהשתלב עם שירות הקצאת המשאבים המשולבים.


