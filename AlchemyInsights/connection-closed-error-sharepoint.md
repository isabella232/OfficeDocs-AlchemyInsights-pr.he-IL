---
title: החיבור שנוהה היה סגור ב- SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317697"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>שגיאת "החיבור שנסגר" ב- SharePoint

אם אתה מקבל את השגיאה "החיבור של בסיס נסגר" ב- SharePoint ייתכן שהוא קשור לפחת של TLS 1.0/1.1. לקבלת מידע נוסף, עיין במאמרים הבאים:

- [הכנה ל-TLS 1.2 ב-Office 365 ו-Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [שגיאות אימות מתרחשות אם ללקוח אין תמיכה ב- TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [עדכן כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

אם המשתמשים נמצאים ב- Windows 7, ודא שהם בודקים [את TLS Cipher Suites ב- Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).