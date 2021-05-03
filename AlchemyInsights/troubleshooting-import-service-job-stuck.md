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
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="94dac-102">פתרון בעיות במשימה 'ייבוא שירות' תקוע</span><span class="sxs-lookup"><span data-stu-id="94dac-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="94dac-103">אם אתה נתקל בבעיות בייבוא משימות שירות תקועות או נכשלות, בדוק ונסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="94dac-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="94dac-104">סקור את גודל קובץ ה- PST.</span><span class="sxs-lookup"><span data-stu-id="94dac-104">Review the size of of the PST file.</span></span> <span data-ttu-id="94dac-105">הגודל המרבי המומלץ של קובץ PST לייבוא הוא 20GB.</span><span class="sxs-lookup"><span data-stu-id="94dac-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="94dac-106">אם אתה חושד שהדלגת על פריטים עקב נזק, הפעל Scanpst.exe כדי לאבחן ולתקן שגיאות בקבצי PST.</span><span class="sxs-lookup"><span data-stu-id="94dac-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="94dac-107">אם אתה רואה שגיאת "MapiExceptionShutoffQuotaExceed" במהלך הייבוא, ודא שלתיבת הדואר של היעד יש מספיק קיבולת לייבא את קבצי ה- PST הרצויים.</span><span class="sxs-lookup"><span data-stu-id="94dac-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="94dac-108">לקבלת מידע נוסף אודות פתרון בעיות במשימות ייבוא PST, ראה [פתרון בעיות במשימות ייבוא של PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="94dac-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="94dac-109">לקבלת מידע אודות פתרון בעיות בעת ייבוא קבצי PSTs Outlook, ראה פתרון בעיות בייבוא [קובץ .pst Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="94dac-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>