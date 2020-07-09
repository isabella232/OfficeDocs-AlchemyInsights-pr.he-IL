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
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="8f32b-102">בעיית ההדפסה ברקע נפתרה</span><span class="sxs-lookup"><span data-stu-id="8f32b-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="8f32b-103">אם ההתקן שלך עודכן באמצעות Windows 10 **OS Build 19041.329**, ייתכן שהבחנת בבעיה שבה מדפסות מסוימות אינן מדפיסות.</span><span class="sxs-lookup"><span data-stu-id="8f32b-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="8f32b-104">מנגנון ההדפסה ברקע עשוי לבצע שגיאה או להיסגר באופן לא צפוי בעת ניסיון להדפיס, ולא מגיע פלט מהמדפסת המושפעת.</span><span class="sxs-lookup"><span data-stu-id="8f32b-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="8f32b-105">בעיה זו נפתרה ב-OS לבנות **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="8f32b-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="8f32b-106">**חקירה שוטפת**</span><span class="sxs-lookup"><span data-stu-id="8f32b-106">**Ongoing investigation**</span></span>

<span data-ttu-id="8f32b-107">ייתכן שקובץ שירות מערכת המשנה של רשות האבטחה המקומית (LSASS) **Isass.exe** ייכשל בחלק מההתקנים עם הודעת השגיאה, "תהליך מערכת קריטי, C:\WINDOWS\system32\Isass.exe נכשל עם קוד מצב c0000008.</span><span class="sxs-lookup"><span data-stu-id="8f32b-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="8f32b-108">כעת יש להפעיל מחדש את המחשב ".</span><span class="sxs-lookup"><span data-stu-id="8f32b-108">The machine must now be restarted".</span></span>  <span data-ttu-id="8f32b-109">**Microsoft פועלת ברזולוציה ותספק עדכון במהדורה הקרובה.**</span><span class="sxs-lookup"><span data-stu-id="8f32b-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="8f32b-110">לקבלת מידע נוסף, אנא בדוק את [Windows 10 גירסה 2004 בעיות ידועות](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="8f32b-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>