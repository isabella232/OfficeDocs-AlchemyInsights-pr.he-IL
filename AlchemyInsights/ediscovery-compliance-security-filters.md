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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727224"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="c0309-102">אין תוצאות המוחזרות במהלך חיפוש תוכן/ייצוא</span><span class="sxs-lookup"><span data-stu-id="c0309-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="c0309-103">אם אתה נתקל בבעיות בתרחישים הבאים של גילוי אלקטרוני:</span><span class="sxs-lookup"><span data-stu-id="c0309-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="c0309-104">חיפוש תוכן/ייצוא מחזיר נתונים או נתונים בלתי צפויים</span><span class="sxs-lookup"><span data-stu-id="c0309-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="c0309-105">חיפוש הגילוי אלקטרוני או הייצוא נכשלים</span><span class="sxs-lookup"><span data-stu-id="c0309-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="c0309-106">ייתכן שהסיבה לכך היא מסנני אבטחה מסוימים המוגדרים על-ידי מנהל מערכת ספציפי ושאינם מועברים לכל מנהלי המערכת.</span><span class="sxs-lookup"><span data-stu-id="c0309-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="c0309-107">כדי לפתור זאת, בדוק אם קיימים מסנני אבטחה של תאימות שעשויים לגרום לבעיות אלה:</span><span class="sxs-lookup"><span data-stu-id="c0309-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="c0309-108">התחברות למרכז האבטחה והתאימות של Powershell</span><span class="sxs-lookup"><span data-stu-id="c0309-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="c0309-109">הפעלת הcommandlet הבאים:</span><span class="sxs-lookup"><span data-stu-id="c0309-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="c0309-110">לקבלת מידע נוסף אודות מסנני אבטחה של תאימות, ראה [סינון הרשאות עבור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="c0309-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
