---
title: בעיות עם SharePoint ב- Windows 7 מחשבים
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125121"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>בעיות עם SharePoint ב- Windows 7 מחשבים

אם אתה מקבל שגיאות ב- Windows 7 מחשבים במהלך העבודה על SharePoint או OneDrive, ייתכן שהן קשורות לפחת של TLS 1.0/1.1. לקבלת מידע נוסף, ראה:

- [הכנה ל-TLS 1.2 ב-Office 365 ו-Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 לקוחות צריכים להיות זמינים ב- TLS1.2. לקבלת מידע נוסף, [ראה שגיאות אימות מתרחשות כאשר ללקוח אין תמיכה ב- TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- התקן את KB3140245 וצור את ערך הרישום. לקבלת מידע נוסף, ראה [עדכון כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows

- Windows 7 SP1/Windows 8 חייבים לוודא שסוויטות הצופן העדכניות ביותר של TLS מותקנות. לקבלת מידע נוסף, ראה [עלון יידוע בנושא אבטחה של Microsoft מס' 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


