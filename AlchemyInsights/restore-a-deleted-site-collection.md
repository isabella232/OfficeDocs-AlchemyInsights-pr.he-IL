---
title: שחזור אתר שנמחק
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768549"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="d6b9b-102">שחזור אתר שנמחק</span><span class="sxs-lookup"><span data-stu-id="d6b9b-102">Restore a deleted site</span></span>

<span data-ttu-id="d6b9b-103">כאשר admin מוחק אתר SharePoint, הוא ממוקם בסל המיחזור של אוסף האתרים, שבו הוא נשמר במשך 93 ימים לפני שהוא נמחק לצמיתות.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="d6b9b-104">כדי לשחזר את האתר:</span><span class="sxs-lookup"><span data-stu-id="d6b9b-104">To restore the site:</span></span>
  
1. <span data-ttu-id="d6b9b-105">במרכז הניהול החדש של SharePoint, לחץ על **סל המיחזור** ברצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d6b9b-106">בחר בתיבת הסימון לצד אוסף האתרים שברצונך לשחזר.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d6b9b-107">לחץ על **שחזר פריטים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d6b9b-108">כדי לשחזר אתר תקשורת שנמחק, באפשרותך להשתמש במרכז הניהול החדש של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="d6b9b-109">אחרת, עליך להשתמש ב-Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="d6b9b-110">כדי לשחזר אתר השייך לקבוצת Office 365, עליך לשחזר את הקבוצה במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="d6b9b-111">ניתן לשחזר קבוצות במשך 30 יום לאחר מחיקתם.</span><span class="sxs-lookup"><span data-stu-id="d6b9b-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

