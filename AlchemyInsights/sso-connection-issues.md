---
title: בעיות בחיבור SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935114"
---
# <a name="sso-connection-issues"></a>בעיות בחיבור SSO

1. פעל בהתאם [לתחלה: קביעת תצורה של מאפיינים עבור מדריך יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) כדי לקבוע את תצורת היישום שלך.
2. בהתאם לאפשרות היישום [וכניסה יחידה](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) שבחרת, בצע את ההנחיות המתאימות להלן:
    - כדי לקבוע תצורה של **יישום מקומי** עבור **כניסה יחידה מבוססת SAML**, ראה [SAML כניסה יחידה עבור יישומים מקומיים באמצעות Proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - כדי לקבוע תצורה של **יישום ענן** עבור **כניסה יחידה מבוססת סיסמה**, ראה  [קביעת תצורה של כניסה יחידה באמצעות](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)סיסמה.
    - כדי לקבוע תצורה של **יישום מקומי** עבור **כניסה יחידה באמצעות proxy של יישום**, ראה [מקומר סיסמה עבור כניסה יחידה באמצעות proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **פתרון בעיות של Proxy של יישומים**: אנו ממליצים לך להתחיל בסקירת זרימת פתרון [הבעיות, בעיות במחברי Proxy של יישומי proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), כדי לקבוע אם מחברים של יישומי proxy מוגדרים כראוי. אם אתה עדיין נתקל בבעיות בהתחברות ליישום, בצע את זרימת פתרון [הבעיות בנושא בעיות ביישום Proxy של יישומי Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). באפשרותך [לזהות בעיות](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ב-CORS באמצעות כלי איתור באגים בדפדפן:
    - הפעל את הדפדפן ואתר את יישום האינטרנט.
    - הקש **F12** כדי להעלות את מסוף איתור הבאגים.
    - נסה לשחזר את הטרנזקציה וסקור את הודעת המסוף. הפרה של CORS מפיקה שגיאת מסוף לגבי המקור.
    - לא ניתן לפתור בעיות מסוימות ב-CORS, כגון כאשר האפליקציה מנתבת מחדש ל-login.microsoft.com כדי לבצע אימות, והאסימון של access פג. לאחר מכן, השיחה של CORS נכשלת. פתרון עבור תרחיש זה הוא להאריך את משך החיים של אסימון הגישה, כדי למנוע ממנו לפוג במהלך הפעלת משתמש. לקבלת מידע נוסף אודות האופן שבו ניתן לעשות זאת, ראה [אורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **פתרון בעיות כניסה יחידה מבוססת SAML: מומלץ** לבדוק [בעיות בכניסה ליישומים המוגדרים כניסה יחידה של SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), כדי למצוא את הפתרונות לבעיות שבהן אתה עשוי להיתקל.
5. **פתרון בעיות כניסה יחידה מבוססת סיסמה**: אנו ממליצים לבדוק [בעיות כניסה יחידה מבוססת סיסמה בתכלת לספירה](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), כדי למצוא את הפתרונות לבעיות שבהן אתה עשוי להיתקל.
6. לקבלת בעיות חיבור בעת שימוש ב-VPN, ראה [כיצד להשתמש בכניסה יחידה (SSO) דרך vpn וWi-Fi חיבורים](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
