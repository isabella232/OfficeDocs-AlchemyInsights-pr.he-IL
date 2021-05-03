---
title: פתרון בעיות במשימה 'ייבוא שירות' תקוע
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125109"
---
# <a name="troubleshooting-import-service-job-stuck"></a>פתרון בעיות במשימה 'ייבוא שירות' תקוע

אם אתה נתקל בבעיות בייבוא משימות שירות תקועות או נכשלות, בדוק ונסה את הפעולות הבאות:

- סקור את גודל קובץ ה- PST. הגודל המרבי המומלץ של קובץ PST לייבוא הוא 20GB.

- אם אתה חושד שהדלגת על פריטים עקב נזק, הפעל Scanpst.exe כדי לאבחן ולתקן שגיאות בקבצי PST.

- אם אתה רואה שגיאת "MapiExceptionShutoffQuotaExceed" במהלך הייבוא, ודא שלתיבת הדואר של היעד יש מספיק קיבולת לייבא את קבצי ה- PST הרצויים.

לקבלת מידע נוסף אודות פתרון בעיות במשימות ייבוא PST, ראה [פתרון בעיות במשימות ייבוא של PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

לקבלת מידע אודות פתרון בעיות בעת ייבוא קבצי PSTs Outlook, ראה פתרון בעיות בייבוא [קובץ .pst Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).