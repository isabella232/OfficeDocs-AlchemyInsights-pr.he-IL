---
title: סינכרון פרופילים
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801770"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5d7eb-102">מתי הפרופיל שלי משתנה ליישום פרופיל המשתמש של SharePoint?</span><span class="sxs-lookup"><span data-stu-id="5d7eb-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5d7eb-103">SharePoint Online משתמש במשימת הטיימר המיובאת של Active Directory (ייבוא AD) כדי לייבא משתמשים וקבוצות ליישום פרופילי משתמשים.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5d7eb-104">AD Import מסנכרן שינויים מחנות הספריות של SharePoint Online ליישום פרופילי משתמשים.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="5d7eb-105">שינויים אלה מעובדים באצוות.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5d7eb-106">משימת שעון העצר פועלת עד לסינכרון השינויים.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5d7eb-107">הזמן הדרוש להפעלת המשימה תלוי במספר השינויים לתהליך.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="5d7eb-108">מספר גדול של שינויים אורכים זמן רב יותר.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-108">A large number of changes takes longer.</span></span> <span data-ttu-id="5d7eb-109">הסכם רמת שירות (SLA) מציין ששינוי למשתמש במדריך הכתובות של SharePoint Online ישתקף ביישום פרופיל המשתמש תוך 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="5d7eb-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5d7eb-110">מידע נוסף אודות סינכרון פרופילי משתמשים ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5d7eb-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

