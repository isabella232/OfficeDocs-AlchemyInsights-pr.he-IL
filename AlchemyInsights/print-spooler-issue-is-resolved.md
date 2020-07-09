---
title: בעיית ההדפסה ברקע נפתרה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088338"
---
# <a name="print-spooler-issue-is-resolved"></a>בעיית ההדפסה ברקע נפתרה

אם ההתקן שלך עודכן באמצעות Windows 10 **OS Build 19041.329**, ייתכן שהבחנת בבעיה שבה מדפסות מסוימות אינן מדפיסות. מנגנון ההדפסה ברקע עשוי לבצע שגיאה או להיסגר באופן לא צפוי בעת ניסיון להדפיס, ולא מגיע פלט מהמדפסת המושפעת. בעיה זו נפתרה ב-OS לבנות **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**חקירה שוטפת**

ייתכן שקובץ שירות מערכת המשנה של רשות האבטחה המקומית (LSASS) **Isass.exe** ייכשל בחלק מההתקנים עם הודעת השגיאה, "תהליך מערכת קריטי, C:\WINDOWS\system32\Isass.exe נכשל עם קוד מצב c0000008. כעת יש להפעיל מחדש את המחשב ".  **Microsoft פועלת ברזולוציה ותספק עדכון במהדורה הקרובה.**

לקבלת מידע נוסף, אנא בדוק את [Windows 10 גירסה 2004 בעיות ידועות](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).