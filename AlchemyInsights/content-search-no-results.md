---
title: חיפוש תוכן ללא תוצאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816849"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="08852-102">אין תוצאות מחיפוש/ייצוא תוכן</span><span class="sxs-lookup"><span data-stu-id="08852-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="08852-103">בעיות בחיפוש/ייצוא תוכן עשויות שלא להחזיר נתונים עקב מסנן אבטחה מסוים של תאימות שהוגנה על-ידי מנהל מערכת ספציפי ולא העברתם לכל מנהלי המערכת.</span><span class="sxs-lookup"><span data-stu-id="08852-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="08852-104">כדי לפתור בעיה זו, בדוק אם זמינים מסנני אבטחה של תאימות שעשויים לגרום לכך:</span><span class="sxs-lookup"><span data-stu-id="08852-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="08852-105">התחברות למרכז האבטחה והתאימות Powershell</span><span class="sxs-lookup"><span data-stu-id="08852-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="08852-106">הפעל את הפקודות הבאות:</span><span class="sxs-lookup"><span data-stu-id="08852-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="08852-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="08852-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="08852-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="08852-108">Get-ComplianceSecurityFilter -Organization $org</span></span>