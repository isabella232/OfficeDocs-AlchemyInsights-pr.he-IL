---
title: פתרון בעיות ב- ediscovery כולל שגיאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676150"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="4a6f9-102">פתרון בעיות ב- ediscovery כולל שגיאות</span><span class="sxs-lookup"><span data-stu-id="4a6f9-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="4a6f9-103">נתקל בבעיות עם החזקות גילוי אלקטרוני?</span><span class="sxs-lookup"><span data-stu-id="4a6f9-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="4a6f9-104">להלן כמה שיטות עבודה מומלצות שיש לשקול:</span><span class="sxs-lookup"><span data-stu-id="4a6f9-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="4a6f9-105">בדוק את מצב ההפצה של החזקה.</span><span class="sxs-lookup"><span data-stu-id="4a6f9-105">Check the hold distribution status.</span></span>  <span data-ttu-id="4a6f9-106">אם המצב פעיל **(ממתין)** או **כבוי (ממתין),** המתן להשלמת התפלגות החזקה.</span><span class="sxs-lookup"><span data-stu-id="4a6f9-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="4a6f9-107">מזג עדכונים של גילוי אלקטרוני לאחסון עדכונים בבקשה בצובר אחת במקום לעדכן את המדיניות שוב ושוב עבור כל טרנזקציה.</span><span class="sxs-lookup"><span data-stu-id="4a6f9-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="4a6f9-108">הפעל Set-CaseHoldPolicy <policyname> -retryDistribution in the Security and Compliance Center Powershell.</span><span class="sxs-lookup"><span data-stu-id="4a6f9-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="4a6f9-109">לקבלת פרטים, [ראה התחברות אל מרכז & תאימות של PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="4a6f9-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="4a6f9-110">לקבלת שלבים כדי לבדוק הגדרות אלה ושיטות עבודה מומלצות נוספות להקלה ופתרון של גילוי אלקטרוני תפתור בעיות, ראה פתרון שגיאות בהמתנה [של גילוי אלקטרוני.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="4a6f9-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="4a6f9-111">לקבלת מידע אודות פתרון בעיות נפוצות אחרות של גילוי אלקטרוני, ראה [חקירה, פתרון בעיות](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)נפוצות של גילוי אלקטרוני ופתרון בעיות נפוצות ב גילוי אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="4a6f9-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
