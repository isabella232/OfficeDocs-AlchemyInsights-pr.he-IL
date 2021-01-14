---
title: בעיות בשילוב של SSO חלק באמצעות היישומים המקומיים שלי
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868678"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>בעיות בשילוב של SSO חלק באמצעות היישומים המקומיים שלי

כדי לפתור בעיות בשילוב של SSO חלק עם יישומים מקומיים, בצע את הפעולות הבאות:

**שלבים מומלצים**

1. כדי לקבוע תצורה של **יישום מקומי** עבור **כניסה יחידה באמצעות proxy של יישום**, ראה [מקומר סיסמה עבור כניסה יחידה באמצעות proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **פתרון בעיות של Proxy של יישומים**: מומלץ להתחיל בסקירת זרימת פתרון [הבעיות, בעיות במחברי Proxy של יישומי proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), כדי לקבוע אם מחברי proxy של יישום מוגדרים כראוי. אם אתה עדיין נתקל בבעיות בהתחברות ליישום, בצע את שלבי פתרון [הבעיות בנושא בעיות ביישום Proxy של יישומי Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). באפשרותך [לזהות בעיות](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ב-CORS באמצעות כלי איתור הבאגים הבאים של הדפדפן:
    1. הפעל את הדפדפן ואתר את יישום האינטרנט.
    1. הקש **F12** כדי להעלות את מסוף איתור הבאגים.
    1. נסה לשחזר את הטרנזקציה וסקור את הודעת המסוף. הפרה של CORS מפיקה שגיאת מסוף לגבי המקור.
    1. לא ניתן לפתור בעיות מסוימות ב-CORS, כגון כאשר האפליקציה מנתבת מחדש ל-login.microsoftonline.com כדי לבצע אימות, והאסימון של access פג. לאחר מכן, השיחה של CORS נכשלת. פתרון עבור תרחיש זה הוא להאריך את משך החיים של אסימון הגישה, כדי למנוע ממנו לפוג במהלך הפעלת משתמש. לקבלת מידע נוסף אודות האופן שבו ניתן לעשות זאת, ראה [אורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**מסמכים מומלצים**

- [כיצד להגדיר כניסה יחידה ליישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML כניסה יחידה עבור יישומים מקומיים עם Proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [הכרת בעיות ביישום Proxy של יישום מדריך כתובות של Active Directory CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [פתרון בעיות של תצורות הקצאה מוגבלת של Kerberos עבור Proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)