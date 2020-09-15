---
title: הדפסת בעיית מנגנון ההדפסה ברקע נפתרה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801842"
---
# <a name="print-spooler-issue-is-resolved"></a>הדפסת בעיית מנגנון ההדפסה ברקע נפתרה

אם המכשיר שלך עודכן ב-Windows 10  **OS גירסת Build**מס ' 19041.329, ייתכן שהבחנת בבעיה שבה מדפסות מסוימות אינן מודפסות. מנגנון ההדפסה ברקע עשוי להשליך שגיאה או לסגור באופן בלתי צפוי בעת ניסיון להדפיס, ואין פלט מגיע מהמדפסת המושפעת. בעיה זו נפתרה במערכת הפעלה של גירסת Build מס '  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**חקירה מתמשכת**

קובץ שירות מערכת המשנה (LSASS) של רשות האבטחה המקומית **Isass.exe** עשוי להיכשל במכשירים מסוימים באמצעות הודעת השגיאה, "תהליך מערכת קריטי, C:\WINDOWS\system32\Isass.exe נכשל עם קוד המצב c0000008. כעת יש להפעיל מחדש את המחשב.  **Microsoft עובדת על פתרון ותספק עדכון במהדורה הבאה.**

לקבלת מידע נוסף, עיין  [בבעיות ידועות ב-Windows 10 גירסה 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).