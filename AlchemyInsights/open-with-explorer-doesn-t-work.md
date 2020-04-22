---
title: הפתיחה באמצעות סייר אינה פועלת
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713035"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="5a5bc-102">הפתיחה באמצעות סייר אינה פועלת</span><span class="sxs-lookup"><span data-stu-id="5a5bc-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="5a5bc-103">אם **הפתיחה באמצעות סייר** או **תצוגה ב-Explorer של הקובץ** אינה פועלת, ודא שהשירות webclient מוגדר **לפעולה** על-ידי ביצוע השלבים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="5a5bc-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="5a5bc-104">לדוגמה, ייתכן שייקח זמן רב לפתוח ספריית SharePoint או OneDrive כאשר השירות אינו פועל.</span><span class="sxs-lookup"><span data-stu-id="5a5bc-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="5a5bc-105">בתיבת החיפוש של Windows, הקלד הפעלה, בחר את יישום שולחן העבודה, הקלד services. msc ולאחר מכן בחר באפשרות **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5a5bc-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="5a5bc-106">גלול מטה לשירות WebClient ובדוק את עמודת **המצב** .</span><span class="sxs-lookup"><span data-stu-id="5a5bc-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="5a5bc-107">אם מצב השירות WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="5a5bc-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="5a5bc-108">הפעל את השירות, במידת הצורך, על-ידי בחירה באפשרות **ידני** או **אוטומטי** בתיבה **סוג הפעלה** .</span><span class="sxs-lookup"><span data-stu-id="5a5bc-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5a5bc-109">כדי לפתור בעיות פתיחה בסייר הקבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="5a5bc-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="5a5bc-110">סקור את הסינכרון כחלופה טובה יותר: [סנכרן קבצי SharePoint עם לקוח הסינכרון החדש OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="5a5bc-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

