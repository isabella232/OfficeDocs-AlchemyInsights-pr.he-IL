---
title: Single-Sign עבור התקנים מצורפים של Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050011"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>כניסה יחידה עבור מכשירים מצורפים של Azure Active Directory

אם יש לך סביבת Active Directory (AD) מקומית וברצונך להצטרף למחשבים המצורפים לתחום של AD ל- Azure AD, באפשרותך לבצע זאת על-ידי ביצוע צירוף היברידי של Azure AD. [כיצד לבצע: תכנון יישום ההצטרפות ההיברידי של Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) מספק לך את השלבים הקשורים ליישום צירוף Azure AD היברידי בסביבה שלך.

[קביעת התצורה של התקנים מצורפים של Azure AD עבור Single-Sign לשימוש Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**בעיות אסימון רענון ראשי (PRT)** אסימון רענון ראשי (PRT) הוא ממצא מפתח של אימות Azure AD ב- Windows 10, Windows Server 2016 וגירסאות מתקדמות יותר, מכשירי iOS ו- Android. זהו אסימון אינטרנט של JSON (JWT) שהונפק במיוחד ל- Microsoft first token brokers כדי להפוך כניסה יחידה (SSO) לזמינה בכל היישומים המשמשים במכשירים אלה. [ב מהו אסימון רענון ראשי?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), נספק פרטים לגבי אופן ההנפקה, שימוש ב- PRT ומוגן במכשירי Windows 10 אחרים.

**WamDefaultSet: YES ו- AzureADPrt: YES** שדות אלה מציינים אם המשתמש מאומת בהצלחה ל- Azure AD בעת הכניסה למכשיר. אם הערכים הם **NO**, ייתכן שתאריך היעד שלו הוא:

- מפתח אחסון גרוע ב- TPM המשויך למכשיר בעת הרישום (בדוק את KeySignTest בעת הפעלת הרשאות מלאות).
- מזהה כניסה חלופי
- HTTP Proxy לא נמצא

פתרון בעיות במכשירים באמצעות הפקודה dsregcmd - [מצב SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
