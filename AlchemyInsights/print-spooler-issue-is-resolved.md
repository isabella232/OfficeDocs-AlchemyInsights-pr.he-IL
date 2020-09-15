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
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="4027d-102">הדפסת בעיית מנגנון ההדפסה ברקע נפתרה</span><span class="sxs-lookup"><span data-stu-id="4027d-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="4027d-103">אם המכשיר שלך עודכן ב-Windows 10  **OS גירסת Build**מס ' 19041.329, ייתכן שהבחנת בבעיה שבה מדפסות מסוימות אינן מודפסות.</span><span class="sxs-lookup"><span data-stu-id="4027d-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="4027d-104">מנגנון ההדפסה ברקע עשוי להשליך שגיאה או לסגור באופן בלתי צפוי בעת ניסיון להדפיס, ואין פלט מגיע מהמדפסת המושפעת.</span><span class="sxs-lookup"><span data-stu-id="4027d-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="4027d-105">בעיה זו נפתרה במערכת הפעלה של גירסת Build מס '  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="4027d-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="4027d-106">**חקירה מתמשכת**</span><span class="sxs-lookup"><span data-stu-id="4027d-106">**Ongoing investigation**</span></span>

<span data-ttu-id="4027d-107">קובץ שירות מערכת המשנה (LSASS) של רשות האבטחה המקומית **Isass.exe** עשוי להיכשל במכשירים מסוימים באמצעות הודעת השגיאה, "תהליך מערכת קריטי, C:\WINDOWS\system32\Isass.exe נכשל עם קוד המצב c0000008.</span><span class="sxs-lookup"><span data-stu-id="4027d-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="4027d-108">כעת יש להפעיל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="4027d-108">The machine must now be restarted".</span></span>  <span data-ttu-id="4027d-109">**Microsoft עובדת על פתרון ותספק עדכון במהדורה הבאה.**</span><span class="sxs-lookup"><span data-stu-id="4027d-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="4027d-110">לקבלת מידע נוסף, עיין  [בבעיות ידועות ב-Windows 10 גירסה 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="4027d-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>