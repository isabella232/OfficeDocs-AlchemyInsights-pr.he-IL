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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084347"
---
# <a name="sso-connection-issues"></a>בעיות בחיבור SSO

1. בצע את [התחלה מהירה: קביעת תצורה של מאפיינים עבור מדריך יישום כדי](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) לקבוע את תצורת היישום שלך.
2. בהתאם ליישום [ולאפשרות הכניסה היחידה שבחרת,](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) בצע את ההנחיות המתאימות להלן:
    - כדי לקבוע **תצורה של יישום** מקומי עבור כניסה יחידה **מבוססת SAML,** ראה כניסה יחידה של SAML עבור יישומים מקומיים [באמצעות Proxy של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - כדי לקבוע תצורה **של יישום** ענן **עבור כניסה יחידה מבוססת סיסמה,** ראה  [קביעת תצורה של כניסה יחידה של סיסמה](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - כדי לקבוע תצורה **של יישום מקומי עבור** כניסה יחידה באמצעות Proxy של **יישום,** ראה כספת באמצעות סיסמה עבור כניסה יחידה באמצעות Proxy [של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **פתרון בעיות ב- Proxy של** יישום: מומלץ להתחיל ב סקירת זרימת פתרון הבעיות, בעיות [במחבר Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)של יישום איתור באגים, כדי לקבוע אם מחברים של Proxy של יישום מוגדרים כראוי. אם אתה עדיין נתקל בבעיות בהתחברות ליישום, פעל בהתאם לזרימת פתרון הבעיות בפתרון בעיות ביישום [Proxy של יישום איתור באגים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). באפשרותך לזהות [בעיות CORS באמצעות](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) כלי איתור באגים בדפדפן:
    - הפעל את הדפדפן ועיין אל יישום האינטרנט.
    - הקש **F12** כדי להעלות את מסוף איתור הבאגים.
    - נסה לשחזר את התנועה ו לסקור את הודעת הקונסולה. הפרת CORS מפיקה שגיאת קונסולה לגבי המקור.
    - לא ניתן לפתור בעיות CORS מסוימות, כגון כאשר היישום שלך מנתב מחדש login.microsoft.com לאימות, ופג תוקפו של אסימון הגישה. השיחה CORS לאחר מכן נכשלת. פתרון עבור תרחיש זה הוא הארכת משך החיים של אסימון הגישה, כדי למנוע ממנו לפוג במהלך הפעלה של משתמש. לקבלת מידע נוסף אודות אופן פעולה זו, ראה משך חיים [של אסימון הניתן להגדרה ב- פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. פתרון בעיות בכניסה יחידה **מבוססת SAML**: מומלץ לבדוק בעיות בכניסה ליישומים המוגדרים [על-ידי SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)כדי למצוא את הפתרונות לבעיות ש סביר ביותר שתיתקל בהן.
5. פתרון בעיות של כניסה יחידה **מבוססת סיסמה:** מומלץ לבדוק פתרון בעיות כניסה יחידה [מבוססת סיסמה ב- Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), כדי למצוא את הפתרונות לבעיות ש סביר ביותר שתיתקל בהן.
6. עבור בעיות חיבור בעת שימוש ב- VPN, ראה כיצד להשתמש בהתחברות [יחידה (SSO) דרך VPN Wi-Fi חיבורים](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
