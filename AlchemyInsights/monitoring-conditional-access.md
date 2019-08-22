---
title: פיקוח על Access מותנה
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538746"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="bb8e8-102">פיקוח על Access מותנה עבור Exchange</span><span class="sxs-lookup"><span data-stu-id="bb8e8-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="bb8e8-103">משתמשים ייעודיים עם גישה מותנית יקבלו של הודעת דואר אלקטרוני אם הן אינן עונות על דרישות גישה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="bb8e8-104">כדי לפתור זאת, אנו ממליצים אחת או יותר מן הפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="bb8e8-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="bb8e8-105">אם ההתקן הוא presumed כדי להיות שנרשמו, ליידע את המשתמש כדי לעבור אל היישום פורטל החברה ולוודא שהוא יופיע בפורטל החברה.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="bb8e8-106">אם לא, המשתמש צריך לרשום את ההתקן.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="bb8e8-107">בפורטל תכלת הרקיע לעבור אל **Intune \> תאימות ההתקן**.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bb8e8-108">תחת **הצג** , לחץ על **תאימות ההתקן**.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="bb8e8-109">הצג את הדוח תאימות ההתקן כדי לאמת את ההתקן של המשתמש מסומן באופן תואם.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="bb8e8-110">בפורטל תכלת הרקיע לעבור אל **Intune \> תאימות ההתקן**.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bb8e8-111">תחת **ניהול**, לחץ על **פריטי מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="bb8e8-112">ברשימה של מדיניות תאימות, ודא פרופיל מוקצית להתקן של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="bb8e8-113">אם לא קיים פרופיל מוקצה, Intune לא יוכלו לאשר מצב תאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="bb8e8-114">ערוך את ההקצאה של access מותנה של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="bb8e8-115">בפורטל תכלת הרקיע לעבור אל **Intune \> גישה מותנית \> מדיניות**</span><span class="sxs-lookup"><span data-stu-id="bb8e8-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="bb8e8-116">בחר מדיניות מהרשימה</span><span class="sxs-lookup"><span data-stu-id="bb8e8-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="bb8e8-117">לחץ על **משתמשים וקבוצות**</span><span class="sxs-lookup"><span data-stu-id="bb8e8-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="bb8e8-118">כדי לייעד מדיניות מסוימים בכל אדם, להוסיף אותן לרשימת **הכלילה** .</span><span class="sxs-lookup"><span data-stu-id="bb8e8-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="bb8e8-119">כדי להבטיח כי אדם מושמט מן המדיניות, להוסיף אותם לרשימת **אי-כלילה** .</span><span class="sxs-lookup"><span data-stu-id="bb8e8-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="bb8e8-120">קרא עוד: [כיצד Access מותנה צג התקנים](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="bb8e8-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

