---
title: פתח באמצעות הסייר אינו פועל
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291716"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="7b884-102">פתח באמצעות הסייר אינו פועל</span><span class="sxs-lookup"><span data-stu-id="7b884-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="7b884-p101">אם **פתח באמצעות סייר** או **תצוגה ב- Explorer קובץ** אינה פועלת ודא כי שירות WebClient מוגדר **פועל** על-ידי ביצוע השלבים הבאים. לדוגמה, היא עשויה להימשך זמן רב כדי לפתוח ספריית SharePoint או OneDrive כאשר השירות אינו פועל.</span><span class="sxs-lookup"><span data-stu-id="7b884-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="7b884-105">בתיבת החיפוש של Windows, סוג הפעלה, בחר את הפעל app שולחן העבודה, סוג services. msc ולאחר מכן בחר **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7b884-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="7b884-p102">גלול מטה אל שירות WebClient ובדוק את עמודה **מצב** . אם המצב שירות WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**. הפעל את השירות, במידת הצורך, על-ידי בחירה **ידנית** או **אוטומטית** בתיבה **סוג הפעלה** .</span><span class="sxs-lookup"><span data-stu-id="7b884-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="7b884-p103">כדי לפתור בעיות בפתיחת בסייר קבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665). סיור סינכרון בתור חלופה טובה יותר: [SharePoint סינכרון קבצים עם לקוח סינכרון OneDrive החדש](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="7b884-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

