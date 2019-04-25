---
title: פתרון בעיות באמצעות פתח באמצעות סייר
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390608"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="4dd81-102">פתור בעיות הקשורות פתח באמצעות סייר</span><span class="sxs-lookup"><span data-stu-id="4dd81-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="4dd81-103">פתור בעיות נפוצות עם פתיחת ספריית מסמכים ב- SharePoint או OneDrive על-ידי שימוש בפקודה **פתח באמצעות סייר** :</span><span class="sxs-lookup"><span data-stu-id="4dd81-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="4dd81-104">השתמש ב- Internet Explorer 10 או 11 של Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="4dd81-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="4dd81-105">**פתח באמצעות סייר** אינו תואם Microsoft קצה, Google Chrome, Firefox ואחרים.</span><span class="sxs-lookup"><span data-stu-id="4dd81-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="4dd81-106">**פתח באמצעות סייר** אינה זמינה בכל הדפדפנים מלבד Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="4dd81-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="4dd81-107">**פתח באמצעות סייר** אינו זמין בחוויית מודרני עבור ספריות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4dd81-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="4dd81-108">במקום זאת, השתמש **בתצוגת סייר הקבצים** .</span><span class="sxs-lookup"><span data-stu-id="4dd81-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="4dd81-109">בחר **אפשרויות תצוגה** \> **תצוגת בסייר הקבצים**.</span><span class="sxs-lookup"><span data-stu-id="4dd81-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="4dd81-110">הצג בסייר הקובץ אינו תואם Microsoft קצה, Google Chrome, Firefox ואחרים.</span><span class="sxs-lookup"><span data-stu-id="4dd81-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="4dd81-111">**הצג בסייר קבצים** בהזמינים רק ב- Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="4dd81-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="4dd81-112">ודא כי שירות WebClient פועל.</span><span class="sxs-lookup"><span data-stu-id="4dd81-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="4dd81-113">בתיבת החיפוש של Windows, סוג הפעלה, בחר app שולחן העבודה של הפעלה, הקלד services. msc ולאחר מכן הקש Enter.</span><span class="sxs-lookup"><span data-stu-id="4dd81-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="4dd81-114">גלול מטה אל שירות WebClient וודא שעמודה **המצב** מציג "פועל".</span><span class="sxs-lookup"><span data-stu-id="4dd81-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="4dd81-115">אם לא, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="4dd81-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="4dd81-116">(ייתכן שיהיה עליך תחילה להפעיל את השירות על-ידי בחירה **ידנית** או **אוטומטית** בתיבה **סוג הפעלה** ).</span><span class="sxs-lookup"><span data-stu-id="4dd81-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4dd81-117">פתיחת ספרייה בסייר הקבצים שימושית אם אתה זקוק להעתיק או להעביר קבצים ותיקיות מרובים לאחר, אך אם ברצונך לעבוד באופן סדיר בספריה, מומלץ לסנכרן אותו.</span><span class="sxs-lookup"><span data-stu-id="4dd81-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="4dd81-118">כדי לפתור בעיות בפתיחת בסייר קבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="4dd81-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="4dd81-119">לקבלת מידע אודות הגדרת סינכרון, ראה [קבצי SharePoint סינכרון עם לקוח סינכרון OneDrive החדש](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="4dd81-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="4dd81-120">נא עיין במאמר [כיצד ניתן להשתמש בפקודה "פתח עם סייר" כדי לפתור בעיות ב- SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="4dd81-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

