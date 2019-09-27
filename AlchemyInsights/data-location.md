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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207262"
---
# <a name="data-location"></a><span data-ttu-id="e4d45-102">מיקום נתונים</span><span class="sxs-lookup"><span data-stu-id="e4d45-102">Data location</span></span>

<span data-ttu-id="e4d45-103">באפשרותך להציג את המיקום של הדייר 365 של Office במרכז הניהול או על-ידי התחברות ל-Exchange Online דרך PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e4d45-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="e4d45-104">**מרכז ניהול:**</span><span class="sxs-lookup"><span data-stu-id="e4d45-104">**Admin center:**</span></span>
1. <span data-ttu-id="e4d45-105">היכנס [למרכז הניהול](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="e4d45-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="e4d45-106">בחר באפשרות **הגדרות** > **פרופיל ארגוני**.</span><span class="sxs-lookup"><span data-stu-id="e4d45-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="e4d45-107">תחת **מיקום נתונים**, בחר באפשרות **הצגת פרטים**.</span><span class="sxs-lookup"><span data-stu-id="e4d45-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="e4d45-108">**PowerShell**</span><span class="sxs-lookup"><span data-stu-id="e4d45-108">**PowerShell:**</span></span>
1. <span data-ttu-id="e4d45-109">התחבר ל-Exchange Online באמצעות Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e4d45-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="e4d45-110">בצע את ה-cmdlet ' [קבל](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) ' של הארגון כדי להציג רשימה של המאפיינים של הדייר.</span><span class="sxs-lookup"><span data-stu-id="e4d45-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="e4d45-111">הבט במאפיין ' מזהה הארגון '.</span><span class="sxs-lookup"><span data-stu-id="e4d45-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="e4d45-112">כאשר יש לך את מיקום הנתונים עבור EXO ו-SPO, באפשרותך לקבוע את מיקום הנתונים עבור שירותים אחרים שבהם אתה עשוי להשתמש [מהיכן שהנתונים שלך ממוקמים](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="e4d45-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>