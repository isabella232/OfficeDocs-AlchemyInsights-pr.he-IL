---
title: סנכרון פרופילים
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768114"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="1949b-102">מתי הפרופיל שלי משתנה ומסונכרן ליישום פרופיל המשתמש של SharePoint?</span><span class="sxs-lookup"><span data-stu-id="1949b-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="1949b-103">SharePoint Online משתמש במשימת שעון העצר Active Directory ייבוא (AD Import) כדי לייבא משתמשים וקבוצות אל יישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1949b-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="1949b-104">AD ייבוא שינויים מסונכרנים מתוך מאגר הספריות המקוונות של SharePoint ליישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1949b-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="1949b-105">שינויים אלה מעובדים בקבוצות.</span><span class="sxs-lookup"><span data-stu-id="1949b-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="1949b-106">משימת שעון העצר מופעלת עד שהשינויים מסונכרנים.</span><span class="sxs-lookup"><span data-stu-id="1949b-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="1949b-107">הזמן שלוקח לעבודה לפעול תלוי במספר השינויים לתהליך.</span><span class="sxs-lookup"><span data-stu-id="1949b-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="1949b-108">מספר גדול של שינויים נמשך זמן רב יותר.</span><span class="sxs-lookup"><span data-stu-id="1949b-108">A large number of changes takes longer.</span></span> <span data-ttu-id="1949b-109">הסכם רמת השירות (SLA) מצהיר ששינוי במשתמש בספריה המקוונת של SharePoint ישתקף ביישום פרופילי המשתמשים בתוך 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="1949b-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="1949b-110">מידע נוסף על הפרופיל משתמש סינכרון ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1949b-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

