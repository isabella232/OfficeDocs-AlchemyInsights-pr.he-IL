---
title: פתרון בעיות באמצעות פתיחה באמצעות סייר
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759693"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="8d65f-102">פתרון בעיות בפתיחה באמצעות סייר</span><span class="sxs-lookup"><span data-stu-id="8d65f-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="8d65f-103">תקן בעיות נפוצות בפתיחת ספריית מסמכים ב-SharePoint או OneDrive באמצעות הפקודה **פתח באמצעות סייר** :</span><span class="sxs-lookup"><span data-stu-id="8d65f-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="8d65f-104">השתמש ב-Internet Explorer 10 או ב-Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="8d65f-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="8d65f-105">**הפתיחה באמצעות סייר** אינה תואמת ל-Microsoft Edge, Google Chrome, Firefox ואחרים.</span><span class="sxs-lookup"><span data-stu-id="8d65f-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8d65f-106">**הפתיחה באמצעות סייר** אינה זמינה בכל הדפדפנים מלבד internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8d65f-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="8d65f-107">**פתיחה באמצעות Explorer** אינה זמינה בחוויה המודרנית עבור ספריות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d65f-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="8d65f-108">**השתמש בתצוגה בסייר הקבצים** במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="8d65f-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="8d65f-109">בחר בתצוגת **אפשרויות** \> תצוגה **בסייר הקבצים**.</span><span class="sxs-lookup"><span data-stu-id="8d65f-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="8d65f-110">התצוגה בסייר הקבצים אינה תואמת ל-Microsoft Edge, ל-Google Chrome, לפיירפוקס ולאחרים.</span><span class="sxs-lookup"><span data-stu-id="8d65f-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8d65f-111">**תצוגה בסייר הקבצים** זמינה רק ב-internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8d65f-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="8d65f-112">ודא שהשירות WebClient פועל.</span><span class="sxs-lookup"><span data-stu-id="8d65f-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="8d65f-113">בתיבת החיפוש של Windows, הקלד הפעלה, בחר את יישום שולחן העבודה, הקלד services. msc ולאחר מכן הקש Enter.</span><span class="sxs-lookup"><span data-stu-id="8d65f-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="8d65f-114">גלול מטה לשירות WebClient וודא שעמודת **המצב** מציגה את המילה "פועל".</span><span class="sxs-lookup"><span data-stu-id="8d65f-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="8d65f-115">אם לא, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="8d65f-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8d65f-116">(ייתכן שיהיה עליך להפוך תחילה את השירות לזמין על-ידי בחירה באפשרות **ידני** או **אוטומטי** בתיבה **סוג הפעלה** .)</span><span class="sxs-lookup"><span data-stu-id="8d65f-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8d65f-117">פתיחת ספריה בסייר הקבצים היא שימושית אם עליך להעתיק או להעביר קבצים ותיקיות מרובים פעם אחת, אך אם ברצונך לעבוד באופן קבוע בספריה, אנו ממליצים לסנכרן אותה.</span><span class="sxs-lookup"><span data-stu-id="8d65f-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="8d65f-118">כדי לפתור בעיות פתיחה בסייר הקבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8d65f-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8d65f-119">לקבלת מידע אודות הגדרת סינכרון, ראה [סינכרון קבצי SharePoint עם לקוח הסינכרון החדש OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8d65f-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="8d65f-120">נא עיין במאמר [כיצד להשתמש בפקודה "פתח עם סייר" כדי לפתור בעיות ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="8d65f-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

