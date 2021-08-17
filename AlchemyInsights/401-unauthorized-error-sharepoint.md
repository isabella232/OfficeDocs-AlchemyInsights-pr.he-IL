---
title: 401 שגיאה לא מורשית SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890267"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 שגיאה לא מורשית SharePoint

אם אתה מקבל את השגיאה "(401) לא מורשה" ב- SharePoint ייתכן שהיא קשורה לפחת של TLS 1.0/1.1. לקבלת מידע נוסף, ראה:

- [הכנה ל-TLS 1.2 ב-Office 365 ו-Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [שגיאות אימות מתרחשות אם ללקוח אין תמיכה ב- TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [עדכן כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים כפרוטוקולים מאובטחים המוגדרים כברירת מחדל ב- WinHTTP ב- Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

אם המשתמשים נמצאים ב- Windows 7, ודא שהם בודקים [את TLS Cipher Suites ב- Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).