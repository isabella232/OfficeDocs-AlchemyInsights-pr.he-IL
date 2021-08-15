---
title: פתרון בעיות כניסה יחידה עבור מכשירים מצורפים של Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039247"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>פתרון בעיות כניסה יחידה עבור מכשירים מצורפים של Azure AD

אם יש לך סביבת Active Directory (AD) מקומית וברצונך להצטרף למחשבים המצורפים לתחום של AD ל- Azure AD, באפשרותך לבצע זאת על-ידי ביצוע צירוף היברידי של Azure AD. [כיצד לבצע: תכנון יישום ההצטרפות ההיברידי של Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) מספק לך את השלבים הקשורים ליישום צירוף Azure AD היברידי בסביבה שלך.

לקבלת מידע נוסף, ראה [קביעת תצורה של מכשירים מצורפים של Azure AD עבור Single-Sign לשימוש ב- Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**בעיות אסימון רענון ראשי (PRT)**

אסימון רענון ראשי (PRT) הוא ממצא מפתח של אימות Azure AD ב- Windows 10, Windows Server 2016 וגירסאות מתקדמות יותר, מכשירי iOS ו- Android. זהו אסימון אינטרנט של JSON (JWT) שהונפק במיוחד ל- Microsoft first token brokers כדי להפוך כניסה יחידה (SSO) לזמינה בכל היישומים המשמשים במכשירים אלה. לקבלת פרטים אודות אופן ההנפקה, שימוש והגנה של PRT במכשירי Windows 10, ראה [מהו אסימון רענון ראשי?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES ו- AzureADPrt: YES**

שדות אלה מציינים אם המשתמש מאומת בהצלחה ל- Azure AD בעת הכניסה למכשיר. אם הערכים הם **לא**, ייתכן שהערך הוא:

- מפתח אחסון גרוע ב- TPM המשויך למכשיר בעת הרישום (בדוק את KeySignTest בעת הפעלת הרשאות מלאות)
- מזהה כניסה חלופי
- HTTP Proxy לא נמצא

כדי לפתור בעיות במכשירים באמצעות הפקודה dsregcmd, ראה [מצב SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
