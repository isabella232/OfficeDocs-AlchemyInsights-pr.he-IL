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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800378"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="cccfe-102">אין תוצאות מתוך תוכן החיפוש/ייצוא</span><span class="sxs-lookup"><span data-stu-id="cccfe-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="cccfe-103">בעיות עם תוכן החיפוש/ייצוא אינה מחזירה נתונים עשוי לנבוע מסנן אבטחה מסוימים תאימות שהיה ההתקנה על-ידי Admin ספציפיים והעברה לא אותה על כל המנהלים.</span><span class="sxs-lookup"><span data-stu-id="cccfe-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="cccfe-104">כדי לפתור בעיה זו, בדוק אם ישנם מסננים אבטחה תאימות עלולות לגרום זו:</span><span class="sxs-lookup"><span data-stu-id="cccfe-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="cccfe-105">להתחבר Powershell מרכז תאימות ואבטחה</span><span class="sxs-lookup"><span data-stu-id="cccfe-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="cccfe-106">הפעל את commandlets הבאות:</span><span class="sxs-lookup"><span data-stu-id="cccfe-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="cccfe-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="cccfe-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="cccfe-108">Get-ComplianceSecurityFilter-$org של הארגון</span><span class="sxs-lookup"><span data-stu-id="cccfe-108">Get-ComplianceSecurityFilter -Organization $org</span></span>