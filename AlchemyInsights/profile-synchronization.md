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
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371985"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="d7adc-102">בעת סינכרון השינויים בפרופיל שלי כדי יישום פרופיל המשתמש של SharePoint?</span><span class="sxs-lookup"><span data-stu-id="d7adc-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="d7adc-103">SharePoint Online משתמש משימת שעון העצר Active Directory לייבא (AD ייבוא) כדי לייבא קבוצות ומשתמשים לתוך יישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="d7adc-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="d7adc-104">ייבוא פרסומות יסנכרן שינויים ממאגר ספריה מקוונת SharePoint יישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="d7adc-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="d7adc-105">שינויים אלה מעובדים באצוות.</span><span class="sxs-lookup"><span data-stu-id="d7adc-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="d7adc-106">משימת שעון העצר יפעל עד שהשינויים יסונכרנו.</span><span class="sxs-lookup"><span data-stu-id="d7adc-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="d7adc-107">הזמן שהדרוש להפעלת משימת תלוי מספר שינויים כדי לעבד.</span><span class="sxs-lookup"><span data-stu-id="d7adc-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="d7adc-108">מספר רב של שינויים אורכת זמן רב.</span><span class="sxs-lookup"><span data-stu-id="d7adc-108">A large number of changes takes longer.</span></span> <span data-ttu-id="d7adc-109">הסכם רמת שירות (SLA) מציינת כי שינוי משתמש בספריית SharePoint Online יבואו לידי ביטוי ביישום פרופיל המשתמש ב- 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="d7adc-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="d7adc-110">מידע נוסף אודות סינכרון פרופיל משתמש ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d7adc-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

