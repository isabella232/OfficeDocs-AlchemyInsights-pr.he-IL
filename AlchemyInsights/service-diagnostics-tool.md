---
title: כלי אבחון השירות עבור Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595860"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="f9b4b-102">כלי אבחון השירות עבור Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="f9b4b-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="f9b4b-103">Windows Virtual Desktop (WVD) מציע כלי אבחון המאפשר למנהלי מערכת לזהות שגיאות באמצעות ממשק יחיד.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="f9b4b-104">כלי זה מבצע רישום של מידע הקשור לאבחון בכל פעם שמישהו שהוקצה לו תפקיד WVD משתמש ב- WVD.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="f9b4b-105">כל יומן רישום מכיל מידע אודות תפקיד WVD המעורב בפעילות, הודעות השגיאה המופיעות במהלך ההפעלה ומידע אודות הדייר והמשתמש.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="f9b4b-106">ניתן לקבוע את תצורת Azure Log Analytics כדי ללכוד את יומן הפעילות שנוצר על-ידי כלי האבחון על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f9b4b-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="f9b4b-107">יצירת סביבת עבודה של Log Analytics עם פורטל [Azure או](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="f9b4b-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="f9b4b-108">[חבר מחשבי Windows לצג Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="f9b4b-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="f9b4b-109">קבל את מזהה סביבת העבודה ואת המפתח הראשי של סביבת העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="f9b4b-110">אשף ההגדרה זקוק למידע זה כדי להגדיר כראוי את הסוכן ולהבטיח שהוא יוכל לקיים תקשורת עם Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="f9b4b-111">[העברת נתוני אבחון לסביבת העבודה שלך](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="f9b4b-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="f9b4b-112">באפשרותך לדחוף נתוני אבחון מהדייר WVD שלך ל- Log Analytics עבור סביבת העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="f9b4b-113">[זהה ואבחן](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) בעיות פנימיות או חיצוניות ביחס ל- WVD.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="f9b4b-114">לקבלת מידע נוסף אודות קביעת התצורה של כלי אבחון השירות עבור WVD, ראה שימוש ב- Log Analytics עבור תכונת האבחון.</span><span class="sxs-lookup"><span data-stu-id="f9b4b-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>