---
title: חיפוש תוכן ללא תוצאות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680648"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="d729c-102">אין תוצאות מחיפוש תוכן/ייצוא</span><span class="sxs-lookup"><span data-stu-id="d729c-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="d729c-103">בעיות בחיפוש תוכן/הייצוא לא מחזירות נתונים עשויים לנבוע ממסנן אבטחת תאימות מסוים שהיה הגדרה על-ידי מנהל מערכת ספציפי, ולא לקיים תקשורת עם כל מנהלי המערכת.</span><span class="sxs-lookup"><span data-stu-id="d729c-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="d729c-104">כדי לפתור זאת, בדוק אם קיימים מסנני אבטחה של תאימות שעשויים לגרום לכך:</span><span class="sxs-lookup"><span data-stu-id="d729c-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="d729c-105">התחברות למרכז האבטחה והתאימות של Powershell</span><span class="sxs-lookup"><span data-stu-id="d729c-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="d729c-106">הפעלת הcommandlet הבאים:</span><span class="sxs-lookup"><span data-stu-id="d729c-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="d729c-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="d729c-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="d729c-108">Get-ComplianceSecurityFilter-ארגון $org</span><span class="sxs-lookup"><span data-stu-id="d729c-108">Get-ComplianceSecurityFilter -Organization $org</span></span>