---
title: תיקון 0x8004de40 ב- OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649749"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>תיקון 0x8004de40 ב- OneDrive

אם אתה משתמש ב- Windows 7 ומקבל שגיאה זו, עדכן כדי להפוך [את TLS 1.1 ו- TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)לזמינים כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows.

אם אתה משתמש ב- Windows 10, ואתה מקבל הודעת 0x8004de40 ב- OneDrive:

- אתחל מחדש את המחשב המושפע בעת חיבור לתחום Acitve Directory שלך.
- אם אתחול מחדש אינו מתקן את הבעיה, בטל את ההסתהוות ו להצטרף שוב למכשיר שלך מ- Azure AD. 

**הערה:** עליך להיות ברשת הארגונית שלך בעת ביצוע שלבים אלה. אל תבצע שלבים אלה כאשר אינך מחובר לתשתית הארגונית שלך (לדוגמה, במהלך נסיעה). 

1. פתח שורת פקודה עם הרשאות מלאות על-ידי בחירה **באפשרות** התחל , לחץ באמצעות לחצן העכבר **הימני** על שורת הפקודה ולאחר מכן בחר הפעל **כמנהל מערכת**.

1. הקלד *dsregcmd /leave* והקש **Enter**.

1. לאחר ההשלמה, *הקלד dsregcmd /join* והקש **Enter**.

1. לאחר ההשלמה, סגור את שורת הפקודה.

1. אתחל את המחשב והיכנס ל- OneDrive.