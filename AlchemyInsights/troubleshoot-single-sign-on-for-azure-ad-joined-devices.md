---
title: פתרון בעיות בכניסה יחידה עבור מכשירים המצורפים של תכלת לספירה
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036170"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>פתרון בעיות בכניסה יחידה עבור מכשירים המצורפים של תכלת לספירה

אם יש לך סביבת Active Directory מקומית (AD) וברצונך להצטרף למחשבים המצורפים לתחום הפרסום שלך ל-תכלת AD, באפשרותך לבצע זאת על-ידי ביצוע הצטרפות היברידית של תכלת לספירה. [כיצד לבצע את הפעולות הבאות: תכנון היישום ' הצטרפות ל-Active Directory של Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ' מספק לך את השלבים הקשורים ליישום הצטרפות משולבת של תכלת לספירה בסביבה שלך.

לקבלת מידע נוסף, ראה [קביעת תצורה של מכשירים המצורפים של "תכלת לספירה" עבור Single-Sign מקומית בשימוש ב-Windows שלום לעסקים](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**בעיות באסימון רענון ראשי (PRT)**

אסימון רענון ראשי (PRT) הוא פריט מפתח של אימות מודעות מיידיות ב-Windows 10, Windows Server 2016 וגירסאות מתקדמות יותר, iOS ומכשירי Android. זהו אסימון אינטרנט של JSON (JWT) שהונפקו במיוחד לברוקרים של Microsoft first, כדי לאפשר כניסה יחידה (SSO) על-פני היישומים המשמשים במכשירים אלה. לקבלת פרטים על האופן שבו PRT מונפק, משמש ומוגן במכשירי Windows 10, ראה [מהו אסימון רענון ראשי?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: כן ו-AzureADPrt: כן**

שדות אלה מציינים אם המשתמש הצליח לבצע בהצלחה את הודעת התכלת לספירה בעת כניסה למכשיר. אם הערכים הם **לא**, ייתכן שהסיבה לכך היא:

- מפתח אחסון מקולקל ב-TPM המשויך למכשיר בעת רישום (סמן את KeySignTest בעת הפעלת הרשאות מוגברות)
- מזהה כניסה חלופי
- Proxy של HTTP לא נמצא

כדי לפתור בעיות במכשירים באמצעות הפקודה dsregcmd, ראה [מצב SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
