---
title: זיהוי בעיות של Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595859"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="0349b-102">זיהוי בעיות של Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="0349b-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="0349b-103">Windows Virtual Desktop Diagnostics משתמש ב- cmdlet אחד של PowerShell אך מכיל פרמטרים אופציונליים רבים כדי לצמצם ולבודד בעיות.</span><span class="sxs-lookup"><span data-stu-id="0349b-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="0349b-104">כדי להתחיל בעבודה:</span><span class="sxs-lookup"><span data-stu-id="0349b-104">To get started:</span></span> 

1. <span data-ttu-id="0349b-105">הורד ויבא את מודול PowerShell של שולחן העבודה הווירטואלי של Windows.</span><span class="sxs-lookup"><span data-stu-id="0349b-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="0349b-106">לקבלת פרטים, ראה [כלי Cmdlet של Windows Virtual Desktop עבור Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="0349b-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="0349b-107">הפעל את ה- cmdlet הבא כדי להיכנס לחשבון שלך:</span><span class="sxs-lookup"><span data-stu-id="0349b-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="0349b-108">דוגמה: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="0349b-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="0349b-109">**הערה:** כל השאילתות המשתמשות ב- PowerShell חייבות לכלול את הפרמטרים -UserName או -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="0349b-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="0349b-110">לקבלת יכולות ניטור, ראה שימוש [ב- Log Analytics עבור תכונת האבחון](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="0349b-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="0349b-111">כדי לסנן פעילויות אבחון לפי משתמש, הפעל את ה- cmdlet הבא:</span><span class="sxs-lookup"><span data-stu-id="0349b-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="0349b-112">דוגמה: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="0349b-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="0349b-113">יש רשימה של מסננים ש באפשרותך להפעיל כדי לאבחן בעיות.</span><span class="sxs-lookup"><span data-stu-id="0349b-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="0349b-114">כדי ללמוד עוד אודות אבחון בעיות, ראה זיהוי [ואבחון של בעיות בשולחן העבודה הווירטואלי של Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="0349b-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="0349b-115">כדי ללמוד עוד אודות שגיאות נפוצות, ראה [שגיאות נפוצות senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="0349b-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
