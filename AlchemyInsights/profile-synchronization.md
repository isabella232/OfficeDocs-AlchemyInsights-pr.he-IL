---
title: סנכרון פרופילים
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554334"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="877a5-102">מתי הפרופיל שלי משתנה ומסונכרן ליישום פרופיל המשתמש של SharePoint?</span><span class="sxs-lookup"><span data-stu-id="877a5-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="877a5-103">SharePoint Online משתמש במשימת שעון העצר Active Directory ייבוא (AD Import) כדי לייבא משתמשים וקבוצות אל יישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="877a5-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="877a5-104">AD ייבוא שינויים מסונכרנים מתוך מאגר הספריות המקוונות של SharePoint ליישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="877a5-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="877a5-105">שינויים אלה מעובדים בקבוצות.</span><span class="sxs-lookup"><span data-stu-id="877a5-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="877a5-106">משימת שעון העצר מופעלת עד שהשינויים מסונכרנים.</span><span class="sxs-lookup"><span data-stu-id="877a5-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="877a5-107">הזמן שלוקח לעבודה לפעול תלוי במספר השינויים לתהליך.</span><span class="sxs-lookup"><span data-stu-id="877a5-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="877a5-108">מספר גדול של שינויים נמשך זמן רב יותר.</span><span class="sxs-lookup"><span data-stu-id="877a5-108">A large number of changes takes longer.</span></span> <span data-ttu-id="877a5-109">הסכם רמת השירות (SLA) מצהיר ששינוי במשתמש בספריה המקוונת של SharePoint ישתקף ביישום פרופילי המשתמשים בתוך 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="877a5-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="877a5-110">מידע נוסף על הפרופיל משתמש סינכרון ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="877a5-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

