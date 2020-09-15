---
title: האפשרות ' פתח באמצעות Explorer ' אינה פועלת
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694457"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="1e88a-102">האפשרות ' פתח באמצעות Explorer ' אינה פועלת</span><span class="sxs-lookup"><span data-stu-id="1e88a-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="1e88a-103">אם **האפשרות פתח באמצעות סייר** או **תצוגה בסייר הקבצים** אינה פועלת, ודא ששירות WebClient מוגדר **לפעול** על-ידי ביצוע השלבים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="1e88a-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="1e88a-104">לדוגמה, ייתכן שיחלפו זמן רב לפתיחת ספריה של SharePoint או OneDrive כאשר השירות אינו פועל.</span><span class="sxs-lookup"><span data-stu-id="1e88a-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="1e88a-105">בתיבת החיפוש של Windows, הקלד הופעל, בחר את יישום שולחן העבודה, הקלד services. msc ולאחר מכן בחר **Enter**.</span><span class="sxs-lookup"><span data-stu-id="1e88a-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="1e88a-106">גלול מטה אל שירות WebClient ובדוק את העמודה **מצב** .</span><span class="sxs-lookup"><span data-stu-id="1e88a-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="1e88a-107">אם מצב השירות של WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="1e88a-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="1e88a-108">הפוך את השירות לזמין, במידת הצורך, על-ידי בחירה באפשרות **ידני** או **אוטומטי** בתיבה **סוג הפעלה** .</span><span class="sxs-lookup"><span data-stu-id="1e88a-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1e88a-109">כדי לפתור בעיות שנפתחות בסייר הקבצים, ראה [פתח ב-explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="1e88a-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="1e88a-110">גלה את הסינכרון כחלופה טובה יותר: [סנכרן קבצי SharePoint עם לקוח הסינכרון החדש של OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="1e88a-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

