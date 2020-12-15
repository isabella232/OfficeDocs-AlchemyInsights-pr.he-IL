---
title: אין תוצאות המוחזרות במהלך חיפוש תוכן/ייצוא
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678677"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="1ed87-102">אין תוצאות המוחזרות במהלך חיפוש תוכן/ייצוא</span><span class="sxs-lookup"><span data-stu-id="1ed87-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="1ed87-103">אם אתה נתקל בבעיות בתרחישים הבאים של גילוי אלקטרוני:</span><span class="sxs-lookup"><span data-stu-id="1ed87-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="1ed87-104">חיפוש תוכן/ייצוא מחזיר נתונים או נתונים בלתי צפויים</span><span class="sxs-lookup"><span data-stu-id="1ed87-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="1ed87-105">חיפוש הגילוי אלקטרוני או הייצוא נכשלים</span><span class="sxs-lookup"><span data-stu-id="1ed87-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="1ed87-106">ייתכן שהסיבה לכך היא מסנני אבטחה מסוימים המוגדרים על-ידי מנהל מערכת ספציפי ושאינם מועברים לכל מנהלי המערכת.</span><span class="sxs-lookup"><span data-stu-id="1ed87-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="1ed87-107">כדי לפתור זאת, בדוק אם קיימים מסנני אבטחה של תאימות שעשויים לגרום לבעיות אלה:</span><span class="sxs-lookup"><span data-stu-id="1ed87-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="1ed87-108">התחברות למרכז האבטחה והתאימות של Powershell</span><span class="sxs-lookup"><span data-stu-id="1ed87-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="1ed87-109">הפעלת הcommandlet הבאים:</span><span class="sxs-lookup"><span data-stu-id="1ed87-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="1ed87-110">לקבלת מידע נוסף אודות מסנני אבטחה של תאימות, ראה [סינון הרשאות עבור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="1ed87-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
