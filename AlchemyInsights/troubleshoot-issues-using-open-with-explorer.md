---
title: פתרון בעיות באמצעות ' פתח באמצעות סייר '
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659059"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="afc27-102">פתרון בעיות באפשרות ' פתח באמצעות סייר '</span><span class="sxs-lookup"><span data-stu-id="afc27-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="afc27-103">פתור בעיות נפוצות בפתיחת ספריית מסמכים ב-SharePoint או ב-OneDrive באמצעות הפקודה ' **פתח באמצעות Explorer** ':</span><span class="sxs-lookup"><span data-stu-id="afc27-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="afc27-104">השתמש ב-Internet Explorer 10 או ב-Internet explorer 11.</span><span class="sxs-lookup"><span data-stu-id="afc27-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="afc27-105">**האפשרות פתח באמצעות Explorer** אינה תואמת ל-Microsoft Edge, Google Chrome, Firefox ואחרים.</span><span class="sxs-lookup"><span data-stu-id="afc27-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="afc27-106">**האפשרות פתח** ב-explorer אינה זמינה בכל הדפדפנים למעט internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="afc27-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="afc27-107">האפשרות **פתח באמצעות Explorer** אינה זמינה בחוויה המודרנית של ספריות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="afc27-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="afc27-108">**השתמש בתצוגה בסייר הקבצים** במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="afc27-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="afc27-109">בחר תצוגה **אפשרויות תצוגה** \> **בסייר הקבצים**.</span><span class="sxs-lookup"><span data-stu-id="afc27-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="afc27-110">התצוגה בסייר הקבצים אינה תואמת ל-Microsoft Edge, Google Chrome, Firefox ואחרים.</span><span class="sxs-lookup"><span data-stu-id="afc27-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="afc27-111">**הצג בסייר הקבצים** זמין רק ב-Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="afc27-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="afc27-112">ודא ששירות WebClient פועל.</span><span class="sxs-lookup"><span data-stu-id="afc27-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="afc27-113">בתיבת החיפוש של Windows, הקלד הופעל, בחר את יישום שולחן העבודה, הקלד services. msc ולאחר מכן הקש Enter.</span><span class="sxs-lookup"><span data-stu-id="afc27-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="afc27-114">גלול מטה אל שירות WebClient וודא שעמודת **המצב** מציגה "פועל".</span><span class="sxs-lookup"><span data-stu-id="afc27-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="afc27-115">אם לא, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="afc27-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="afc27-116">(ייתכן שיהיה עליך להפעיל תחילה את השירות על-ידי בחירה באפשרות **ידני** או **אוטומטי** בתיבה **סוג הפעלה** .)</span><span class="sxs-lookup"><span data-stu-id="afc27-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="afc27-117">פתיחת ספריה בסייר הקבצים שימושית אם עליך להעתיק או להעביר קבצים ותיקיות מרובים פעם אחת, אך אם ברצונך לעבוד באופן קבוע בספריה, מומלץ לסנכרן אותו.</span><span class="sxs-lookup"><span data-stu-id="afc27-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="afc27-118">כדי לפתור בעיות שנפתחות בסייר הקבצים, ראה [פתח ב-explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="afc27-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="afc27-119">לקבלת מידע אודות הגדרת סינכרון, ראה [סינכרון קבצי SharePoint עם לקוח הסינכרון החדש של OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="afc27-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="afc27-120">עיין במאמר [כיצד להשתמש בפקודה ' פתח באמצעות הסייר ' כדי לפתור בעיות ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="afc27-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

