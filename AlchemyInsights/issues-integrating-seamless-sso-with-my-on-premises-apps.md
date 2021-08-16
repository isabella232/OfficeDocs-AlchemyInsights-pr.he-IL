---
title: בעיות בשילוב SSO חלק עם היישומים המקומיים שלי
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028293"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>בעיות בשילוב SSO חלק עם היישומים המקומיים שלי

כדי לפתור בעיות בשילוב SSO חלק עם יישומים מקומיים, עשה את הפעולות הבאות:

**שלבים מומלצים**

1. כדי לקבוע תצורה **של יישום מקומי עבור** כניסה יחידה באמצעות Proxy של **יישום,** ראה כספת באמצעות סיסמה עבור כניסה יחידה באמצעות Proxy [של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **פתרון בעיות ב- Proxy של** יישום: מומלץ להתחיל לסקור את זרימת פתרון הבעיות, בעיות [במחבר Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)של יישום איתור באגים , כדי לקבוע אם מחברים של Proxy של יישום מוגדרים כראוי. אם אתה עדיין נתקל בבעיות בהתחברות ליישום, בצע את השלבים לפתרון בעיות ביישום איתור באגים [ביישום Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). באפשרותך לזהות [בעיות CORS באמצעות](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) כלי איתור הבאגים הבאים של הדפדפן:
    1. הפעל את הדפדפן ועיין אל יישום האינטרנט.
    1. הקש **F12** כדי להעלות את מסוף איתור הבאגים.
    1. נסה לשחזר את התנועה ו לסקור את הודעת הקונסולה. הפרת CORS מפיקה שגיאת קונסולה לגבי המקור.
    1. לא ניתן לפתור בעיות CORS מסוימות, כגון כאשר היישום שלך מנתב מחדש login.microsoftonline.com כדי לבצע אימות, ותוקף אסימון הגישה פג. השיחה CORS לאחר מכן נכשלת. פתרון עבור תרחיש זה הוא הארכת משך החיים של אסימון הגישה, כדי למנוע ממנו לפוג במהלך הפעלה של משתמש. לקבלת מידע נוסף אודות אופן פעולה זו, ראה משך חיים [של אסימון הניתן להגדרה ב- פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**מסמכים מומלצים**

- [כיצד להגדיר כניסה יחידה ליישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML כניסה יחידה עבור יישומים מקומיים עם Proxy של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [להבין ולפתור בעיות ב- Proxy CORS של יישום Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [פתרון בעיות של תצורות הקצאה מאולצות של Kerberos עבור Proxy של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)