---
title: מיקום נתונים
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627847"
---
# <a name="data-location"></a><span data-ttu-id="e92e8-102">מיקום נתונים</span><span class="sxs-lookup"><span data-stu-id="e92e8-102">Data location</span></span>

<span data-ttu-id="e92e8-103">באפשרותך להציג את המיקום של הדייר 365 של Office במרכז הניהול או על-ידי התחברות ל-Exchange Online דרך PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e92e8-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="e92e8-104">**מרכז ניהול:**</span><span class="sxs-lookup"><span data-stu-id="e92e8-104">**Admin center:**</span></span>
1. <span data-ttu-id="e92e8-105">היכנס [למרכז הניהול](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="e92e8-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="e92e8-106">בחר באפשרות **הגדרות** > **פרופיל ארגוני**.</span><span class="sxs-lookup"><span data-stu-id="e92e8-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="e92e8-107">תחת **מיקום נתונים**, בחר באפשרות **הצגת פרטים**.</span><span class="sxs-lookup"><span data-stu-id="e92e8-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="e92e8-108">**PowerShell**</span><span class="sxs-lookup"><span data-stu-id="e92e8-108">**PowerShell:**</span></span>
1. <span data-ttu-id="e92e8-109">התחבר ל-Exchange Online באמצעות Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e92e8-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="e92e8-110">בצע את ה-cmdlet ' [קבל](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) ' של הארגון כדי להציג רשימה של המאפיינים של הדייר.</span><span class="sxs-lookup"><span data-stu-id="e92e8-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="e92e8-111">הבט במאפיין ' מזהה הארגון '.</span><span class="sxs-lookup"><span data-stu-id="e92e8-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="e92e8-112">כאשר יש לך את מיקום הנתונים עבור EXO ו-SPO, באפשרותך לקבוע את מיקום הנתונים עבור שירותים אחרים שבהם אתה עשוי להשתמש [מהיכן שהנתונים שלך ממוקמים](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="e92e8-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>