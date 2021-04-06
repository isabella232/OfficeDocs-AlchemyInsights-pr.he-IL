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
# <a name="identify-windows-virtual-desktop-issues"></a>זיהוי בעיות של Windows Virtual Desktop

Windows Virtual Desktop Diagnostics משתמש ב- cmdlet אחד של PowerShell אך מכיל פרמטרים אופציונליים רבים כדי לצמצם ולבודד בעיות. כדי להתחיל בעבודה: 

1. הורד ויבא את מודול PowerShell של שולחן העבודה הווירטואלי של Windows. לקבלת פרטים, ראה [כלי Cmdlet של Windows Virtual Desktop עבור Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. הפעל את ה- cmdlet הבא כדי להיכנס לחשבון שלך:
    
    דוגמה: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**הערה:** כל השאילתות המשתמשות ב- PowerShell חייבות לכלול את הפרמטרים -UserName או -ActivityID. לקבלת יכולות ניטור, ראה שימוש [ב- Log Analytics עבור תכונת האבחון](https://go.microsoft.com/fwlink/?linkid=2126847).

כדי לסנן פעילויות אבחון לפי משתמש, הפעל את ה- cmdlet הבא:

דוגמה: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

יש רשימה של מסננים ש באפשרותך להפעיל כדי לאבחן בעיות. כדי ללמוד עוד אודות אבחון בעיות, ראה זיהוי [ואבחון של בעיות בשולחן העבודה הווירטואלי של Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

כדי ללמוד עוד אודות שגיאות נפוצות, ראה [שגיאות נפוצות senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
