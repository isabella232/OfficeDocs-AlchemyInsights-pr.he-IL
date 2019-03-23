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
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753787"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="edc2a-102">שחזור אוסף אתרים שנמחק</span><span class="sxs-lookup"><span data-stu-id="edc2a-102">Restore a deleted site collection</span></span>

<span data-ttu-id="edc2a-103">בעת ניהול מוחק אוסף אתרים קלאסי, הוא מוצב באוסף האתרים סל המיחזור, שבו נשמרת במשך 93 ימים לפני שהיא נמחקת לצמיתות.</span><span class="sxs-lookup"><span data-stu-id="edc2a-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="edc2a-104">כדי לשחזר את אוסף האתרים:</span><span class="sxs-lookup"><span data-stu-id="edc2a-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="edc2a-105">במרכז admin קלאסי של SharePoint, לחץ על ' **סל המיחזור** ' ברצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="edc2a-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="edc2a-106">בחר את תיבת הסימון לצד אוסף האתרים שברצונך לשחזר.</span><span class="sxs-lookup"><span data-stu-id="edc2a-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="edc2a-107">לחץ על **שחזור פריטים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="edc2a-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="edc2a-108">כדי לשחזר אתר תקשורת שנמחק, באפשרותך להשתמש בתצוגה המקדימה של מרכז הניהול של SharePoint חדשה.</span><span class="sxs-lookup"><span data-stu-id="edc2a-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="edc2a-109">אחרת, עליך להשתמש ב- PowerShell.</span><span class="sxs-lookup"><span data-stu-id="edc2a-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="edc2a-110">כדי לשחזר אתר השייך לקבוצת Office 365, עליך לשחזר את הקבוצה במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="edc2a-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="edc2a-111">ניתן לשחזר קבוצות למשך 30 יום לאחר שהם נמחקו.</span><span class="sxs-lookup"><span data-stu-id="edc2a-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

