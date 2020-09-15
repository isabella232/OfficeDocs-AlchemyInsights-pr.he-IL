---
title: ניטור גישה מותנית
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702904"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="734f4-102">ניטור הגישה המותנית עבור Exchange</span><span class="sxs-lookup"><span data-stu-id="734f4-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="734f4-103">משתמשים המיועדים באמצעות גישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="734f4-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="734f4-104">כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="734f4-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="734f4-105">אם יש להעריך את המכשיר, הקפד למשתמש לעבור לאפליקציית הפורטל של החברה ולוודא שהיא מופיעה בפורטל החברה.</span><span class="sxs-lookup"><span data-stu-id="734f4-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="734f4-106">אם היא אינה מופיעה, המשתמש צריך לרשום את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="734f4-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="734f4-107">בפורטל התכלת, עבור אל **כוונון \> תאימות התקן**.</span><span class="sxs-lookup"><span data-stu-id="734f4-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="734f4-108">תחת **צג** , לחץ על **תאימות מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="734f4-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="734f4-109">הצג את דוח תאימות המכשירים כדי לוודא שהתקן המשתמש מסומן כתואם.</span><span class="sxs-lookup"><span data-stu-id="734f4-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="734f4-110">בפורטל התכלת, עבור אל **כוונון \> תאימות התקן**.</span><span class="sxs-lookup"><span data-stu-id="734f4-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="734f4-111">תחת **ניהול**, לחץ על **מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="734f4-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="734f4-112">ברשימת מדיניות התאימות, ודא שהפרופיל מוקצה למכשיר המשתמש שלך.</span><span class="sxs-lookup"><span data-stu-id="734f4-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="734f4-113">אם לא הוקצה פרופיל, האפשרות ' התאמה ' לא תוכל לאשר את מצב התאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="734f4-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="734f4-114">ערוך את הקצאת הגישה המותנית של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="734f4-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="734f4-115">בפורטל ' תכלת ', עבור אל ' **כוונון \> \> מדיניות גישה מותנית** '</span><span class="sxs-lookup"><span data-stu-id="734f4-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="734f4-116">בחירת מדיניות מהרשימה</span><span class="sxs-lookup"><span data-stu-id="734f4-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="734f4-117">לחץ על **משתמשים וקבוצות**</span><span class="sxs-lookup"><span data-stu-id="734f4-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="734f4-118">כדי לייעד מדיניות מסוימת לאדם כלשהו, הוסף אותם לרשימה **כלול** .</span><span class="sxs-lookup"><span data-stu-id="734f4-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="734f4-119">כדי להבטיח שאדם מושמט מהמדיניות, הוסף אותם לרשימת **אי-הכללה** .</span><span class="sxs-lookup"><span data-stu-id="734f4-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="734f4-120">קרא עוד: [כיצד לנטר התקני גישה מותנית](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="734f4-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

