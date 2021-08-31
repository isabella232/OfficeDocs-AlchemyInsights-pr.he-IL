---
title: בעיות בכניסה לאפליקציות Microsoft 365 שלך
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744637"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>בעיות בכניסה יישומי Microsoft 365

הערה: אם אתה משתמש בגירסה קודמת של Windows (לדוגמה, Windows 7 SP1, Windows Server 2008 R2), השתמש בתיקון הקלה כדי [להפוך](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) את TLS 1.2 לזמין כברירת מחדל. לקבלת מידע נוסף, ראה [עדכון כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows.

כדי לפתור בעיות כניסה עם Microsoft 365, נסה את האפשרויות הבאות במחשב המושפע:  

- לקבלת Windows, ראה [המלצות](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) פתרון בעיות כניסה נפוצות
- עבור Mac, [ראה אין באפשרותך להיכנס לאפליקציה Office 2016 עבור Mac שלך](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**עצה** במחשבי Windows, אנו יכולים לאבחן ולפתור עבורך באופן אוטומטי כמה בעיות כניסה נפוצות של Office. הורד והפעל את  **[מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** כדי להשתמש בכלי האוטומטי שלנו.

**הערה:** ביטול אימות מודרני (ADAL) או ניהול חשבון אינטרנט (WAM) לתיקון בעיות כניסה או **הפעלה אינו מומלץ.** אם השגיאות מתרחשות בעת התחברות Microsoft 365 באמצעות Office 2013, [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) ודא שאתה מאפשר אימות מודרני עבור Office הלקוח.

לקבלת פעולות ספציפיות לפתרון בעיות, ראה:

[בעיות חיבור בהתחברות לאחר העדכון ל-Office 2016 גרסה 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[לא ניתן להיכנס לחשבון הארגוני שלך, כגון Office 365, Azure או Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[כיצד לפתור בעיות באפליקציות שאינן דפדפן שאינן יכולות להיכנס ל- Office 365, ל- Azure או ל- Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[שוב ושוב תתבקש לספק אישורים ב- Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)