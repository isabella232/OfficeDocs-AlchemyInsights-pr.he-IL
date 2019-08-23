---
title: אין תוצאות חיפוש של תוכן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516780"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="95895-102">אין תוצאות מתוך תוכן החיפוש/ייצוא</span><span class="sxs-lookup"><span data-stu-id="95895-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="95895-103">בעיות עם תוכן החיפוש/ייצוא אינה מחזירה נתונים עשוי לנבוע מסנן אבטחה מסוימים תאימות שהיה ההתקנה על-ידי Admin ספציפיים והעברה לא אותה על כל המנהלים.</span><span class="sxs-lookup"><span data-stu-id="95895-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="95895-104">כדי לפתור בעיה זו, בדוק אם ישנם מסננים אבטחה תאימות עלולות לגרום זו:</span><span class="sxs-lookup"><span data-stu-id="95895-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="95895-105">להתחבר Powershell מרכז תאימות ואבטחה</span><span class="sxs-lookup"><span data-stu-id="95895-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="95895-106">הפעל את commandlets הבאות:</span><span class="sxs-lookup"><span data-stu-id="95895-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="95895-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="95895-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="95895-108">Get-ComplianceSecurityFilter-$org של הארגון</span><span class="sxs-lookup"><span data-stu-id="95895-108">Get-ComplianceSecurityFilter -Organization $org</span></span>