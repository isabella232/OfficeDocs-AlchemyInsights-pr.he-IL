---
title: סינכרון פרופילים
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554334"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="d41e2-102">בעת סינכרון השינויים בפרופיל שלי כדי יישום פרופיל המשתמש של SharePoint?</span><span class="sxs-lookup"><span data-stu-id="d41e2-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="d41e2-103">SharePoint Online משתמש משימת שעון העצר Active Directory לייבא (AD ייבוא) כדי לייבא קבוצות ומשתמשים לתוך יישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="d41e2-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="d41e2-104">ייבוא פרסומות יסנכרן שינויים ממאגר ספריה מקוונת SharePoint יישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="d41e2-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="d41e2-105">שינויים אלה מעובדים באצוות.</span><span class="sxs-lookup"><span data-stu-id="d41e2-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="d41e2-106">משימת שעון העצר יפעל עד שהשינויים יסונכרנו.</span><span class="sxs-lookup"><span data-stu-id="d41e2-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="d41e2-107">הזמן שהדרוש להפעלת משימת תלוי מספר שינויים כדי לעבד.</span><span class="sxs-lookup"><span data-stu-id="d41e2-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="d41e2-108">מספר רב של שינויים אורכת זמן רב.</span><span class="sxs-lookup"><span data-stu-id="d41e2-108">A large number of changes takes longer.</span></span> <span data-ttu-id="d41e2-109">הסכם רמת שירות (SLA) מציינת כי שינוי משתמש בספריית SharePoint Online יבואו לידי ביטוי ביישום פרופיל המשתמש ב- 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="d41e2-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="d41e2-110">מידע נוסף אודות סינכרון פרופיל משתמש ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d41e2-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

