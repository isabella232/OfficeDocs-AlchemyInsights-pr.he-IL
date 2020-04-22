---
title: ניטור גישה מותנית
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713719"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="569cd-102">ניטור גישה מותנית עבור Exchange</span><span class="sxs-lookup"><span data-stu-id="569cd-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="569cd-103">משתמשים המיועדים לגישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="569cd-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="569cd-104">כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="569cd-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="569cd-105">אם ההתקן משוער לרשום, הודע למשתמש לעבור ליישום פורטל החברה ולוודא שהוא מופיע בפורטל החברה.</span><span class="sxs-lookup"><span data-stu-id="569cd-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="569cd-106">אם לא, על המשתמש לרשום את ההתקן.</span><span class="sxs-lookup"><span data-stu-id="569cd-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="569cd-107">בפורטל התכלת עבור **לתאימות \> התקן Intune**.</span><span class="sxs-lookup"><span data-stu-id="569cd-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="569cd-108">תחת **הצג** לחץ על **תאימות התקן**.</span><span class="sxs-lookup"><span data-stu-id="569cd-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="569cd-109">הצג את דוח תאימות ההתקן כדי לוודא שהתקן המשתמש מסומן כתואם.</span><span class="sxs-lookup"><span data-stu-id="569cd-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="569cd-110">בפורטל התכלת עבור **לתאימות \> התקן Intune**.</span><span class="sxs-lookup"><span data-stu-id="569cd-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="569cd-111">תחת **ניהול**, לחץ על **פריטי מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="569cd-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="569cd-112">ברשימת מדיניות התאימות, ודא שפרופיל מוקצה להתקן המשתמש.</span><span class="sxs-lookup"><span data-stu-id="569cd-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="569cd-113">אם לא הוקצתה פרופיל, Intune לא תהיה אפשרות לאשר את מצב התאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="569cd-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="569cd-114">ערוך את הקצאת הגישה המותנית של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="569cd-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="569cd-115">בפורטל התכלת עבור אל **Intune \> מדיניות \> גישה מותנית**</span><span class="sxs-lookup"><span data-stu-id="569cd-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="569cd-116">בחירת מדיניות מהרשימה</span><span class="sxs-lookup"><span data-stu-id="569cd-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="569cd-117">לחץ על **משתמשים וקבוצות**</span><span class="sxs-lookup"><span data-stu-id="569cd-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="569cd-118">כדי למקד מדיניות מסוימת במישהו, הוסף אותן לרשימת **הכלילה** .</span><span class="sxs-lookup"><span data-stu-id="569cd-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="569cd-119">כדי להבטיח שאדם יושמט מהמדיניות, הוסף אותם לרשימת **הכלילה** .</span><span class="sxs-lookup"><span data-stu-id="569cd-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="569cd-120">קרא עוד: [כיצד לנטר התקני גישה מותנית](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="569cd-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

