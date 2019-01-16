---
title: פיקוח על Access מותנה
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292903"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="1dd0f-102">פיקוח על Access מותנה</span><span class="sxs-lookup"><span data-stu-id="1dd0f-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="1dd0f-p101">משתמשים ייעודיים עם גישה מותנית יקבלו של הודעת דואר אלקטרוני אם הן אינן עונות על דרישות גישה של הארגון שלך. כדי לפתור זאת, אנו ממליצים אחת או יותר מן הפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="1dd0f-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="1dd0f-p102">אם ההתקן הוא presumed כדי להיות שנרשמו, ליידע את המשתמש כדי לעבור אל היישום פורטל החברה ולוודא שהוא יופיע בפורטל החברה. אם לא, המשתמש צריך לרשום את ההתקן.</span><span class="sxs-lookup"><span data-stu-id="1dd0f-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="1dd0f-p103">בפורטל תכלת הרקיע לעבור אל **Intune \> תאימות ההתקן**. תחת **הצג** , לחץ על **תאימות ההתקן**. הצג את הדוח תאימות ההתקן כדי לאמת את ההתקן של המשתמש מסומן באופן תואם.</span><span class="sxs-lookup"><span data-stu-id="1dd0f-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="1dd0f-p104">בפורטל תכלת הרקיע לעבור אל **Intune \> תאימות ההתקן**. תחת **ניהול**, לחץ על **פריטי מדיניות**. ברשימה של מדיניות תאימות, ודא פרופיל מוקצית להתקן של המשתמש. אם לא קיים פרופיל מוקצה, Intune לא יוכלו לאשר מצב תאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="1dd0f-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="1dd0f-114">ערוך את ההקצאה של access מותנה של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1dd0f-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="1dd0f-115">בפורטל תכלת הרקיע לעבור אל **Intune \> גישה מותנית \> מדיניות**</span><span class="sxs-lookup"><span data-stu-id="1dd0f-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="1dd0f-116">בחר מדיניות מהרשימה</span><span class="sxs-lookup"><span data-stu-id="1dd0f-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="1dd0f-117">לחץ על **משתמשים וקבוצות**</span><span class="sxs-lookup"><span data-stu-id="1dd0f-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="1dd0f-p105">כדי לייעד מדיניות מסוימים בכל אדם, להוסיף אותן לרשימת **הכלילה** . כדי להבטיח כי אדם מושמט מן המדיניות, להוסיף אותם לרשימת **אי-כלילה** .</span><span class="sxs-lookup"><span data-stu-id="1dd0f-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="1dd0f-120">קרא עוד: [כיצד Access מותנה צג התקנים](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="1dd0f-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

