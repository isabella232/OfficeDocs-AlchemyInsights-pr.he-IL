---
title: שחזור אתר שנמחק
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582236"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="9ec11-102">שחזור אתר שנמחק</span><span class="sxs-lookup"><span data-stu-id="9ec11-102">Restore a deleted site</span></span>

<span data-ttu-id="9ec11-103">כאשר admin מוחק אתר SharePoint, הוא ממוקם בסל המיחזור של אוסף האתרים, שבו הוא נשמר במשך 93 ימים לפני שהוא נמחק לצמיתות.</span><span class="sxs-lookup"><span data-stu-id="9ec11-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="9ec11-104">כדי לשחזר את האתר:</span><span class="sxs-lookup"><span data-stu-id="9ec11-104">To restore the site:</span></span>
  
1. <span data-ttu-id="9ec11-105">במרכז הניהול החדש של SharePoint, לחץ על **סל המיחזור** ברצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="9ec11-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="9ec11-106">בחר בתיבת הסימון לצד אוסף האתרים שברצונך לשחזר.</span><span class="sxs-lookup"><span data-stu-id="9ec11-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="9ec11-107">לחץ על **שחזר פריטים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="9ec11-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="9ec11-108">כדי לשחזר אתר תקשורת שנמחק, באפשרותך להשתמש במרכז הניהול החדש של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9ec11-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="9ec11-109">אחרת, עליך להשתמש ב-Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ec11-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="9ec11-110">כדי לשחזר אתר השייך לקבוצת Microsoft 365, עליך לשחזר את הקבוצה במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ec11-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="9ec11-111">ניתן לשחזר קבוצות במשך 30 יום לאחר מחיקתם.</span><span class="sxs-lookup"><span data-stu-id="9ec11-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

