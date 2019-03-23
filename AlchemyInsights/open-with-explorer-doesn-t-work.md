---
title: פתח באמצעות הסייר אינו פועל
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764909"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8c102-102">פתח באמצעות הסייר אינו פועל</span><span class="sxs-lookup"><span data-stu-id="8c102-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8c102-103">אם **פתח באמצעות סייר** או **תצוגה ב- Explorer קובץ** אינה פועלת ודא כי שירות WebClient מוגדר **פועל** על-ידי ביצוע השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="8c102-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8c102-104">לדוגמה, היא עשויה להימשך זמן רב כדי לפתוח ספריית SharePoint או OneDrive כאשר השירות אינו פועל.</span><span class="sxs-lookup"><span data-stu-id="8c102-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8c102-105">בתיבת החיפוש של Windows, סוג הפעלה, בחר את הפעל app שולחן העבודה, סוג services. msc ולאחר מכן בחר **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8c102-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8c102-106">גלול מטה אל שירות WebClient ובדוק את עמודה **מצב** .</span><span class="sxs-lookup"><span data-stu-id="8c102-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8c102-107">אם המצב שירות WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="8c102-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8c102-108">הפעל את השירות, במידת הצורך, על-ידי בחירה **ידנית** או **אוטומטית** בתיבה **סוג הפעלה** .</span><span class="sxs-lookup"><span data-stu-id="8c102-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8c102-109">כדי לפתור בעיות בפתיחת בסייר קבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8c102-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8c102-110">סיור סינכרון בתור חלופה טובה יותר: [SharePoint סינכרון קבצים עם לקוח סינכרון OneDrive החדש](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8c102-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

