---
title: שחזור אוסף אתרים שנמחק
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 22fb513771abc1a604a347204bac268771cb9e37
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939997"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="7f223-102">שחזור אוסף אתרים שנמחק</span><span class="sxs-lookup"><span data-stu-id="7f223-102">Restore a deleted site collection</span></span>

<span data-ttu-id="7f223-p101">בעת ניהול מוחק אוסף אתרים קלאסי, הוא מוצב באוסף האתרים סל המיחזור, שבו נשמרת במשך 93 ימים לפני שהיא נמחקת לצמיתות. כדי לשחזר את אוסף האתרים:</span><span class="sxs-lookup"><span data-stu-id="7f223-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="7f223-105">במרכז admin קלאסי של SharePoint, לחץ על ' **סל המיחזור** ' ברצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="7f223-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="7f223-106">בחר את תיבת הסימון לצד אוסף האתרים שברצונך לשחזר.</span><span class="sxs-lookup"><span data-stu-id="7f223-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="7f223-107">לחץ על **שחזור פריטים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="7f223-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="7f223-p102">כדי לשחזר אתר תקשורת שנמחק, באפשרותך להשתמש בתצוגה המקדימה של מרכז הניהול של SharePoint חדשה. אחרת, עליך להשתמש ב- PowerShell. כדי לשחזר אתר השייך לקבוצת Office 365, עליך לשחזר את הקבוצה במרכז הניהול של Exchange. ניתן לשחזר קבוצות למשך 30 יום לאחר שהם נמחקו.</span><span class="sxs-lookup"><span data-stu-id="7f223-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

