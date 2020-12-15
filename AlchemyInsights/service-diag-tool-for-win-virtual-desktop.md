---
title: כלי אבחון שירות עבור שולחן העבודה של Windows Virtual
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678621"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b07c6-102">כלי אבחון שירות עבור שולחן העבודה של Windows Virtual</span><span class="sxs-lookup"><span data-stu-id="b07c6-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b07c6-103">שולחן העבודה של Windows Virtual (WVD) מציע כלי אבחון המאפשר למנהלי מערכת לזהות שגיאות באמצעות ממשק יחיד.</span><span class="sxs-lookup"><span data-stu-id="b07c6-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b07c6-104">כלי זה מבצע רישום של מידע הקשור לאבחון כאשר WVD נמצא בשימוש על-ידי משתמש שהוקצה לו תפקיד WVD.</span><span class="sxs-lookup"><span data-stu-id="b07c6-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b07c6-105">כל יומן מכיל מידע על תפקיד WVD המעורב בפעילות, הודעות השגיאה המופיעות במהלך ההפעלה והמידע אודות הדייר והמשתמש.</span><span class="sxs-lookup"><span data-stu-id="b07c6-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b07c6-106">ניתן לקבוע את התצורה של ניתוח יומן הרישום של תכלת כדי ללכוד את יומן הפעילות שנוצר על-ידי כלי האבחון.</span><span class="sxs-lookup"><span data-stu-id="b07c6-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="b07c6-107">כך ניתן לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="b07c6-107">Here's how:</span></span>

1. <span data-ttu-id="b07c6-108">צור סביבת עבודה של ניתוח יומני רישום עם [הפורטל ' תכלת](https://go.microsoft.com/fwlink/?linkid=2129500) ' או ' [תכלת PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)'.</span><span class="sxs-lookup"><span data-stu-id="b07c6-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="b07c6-109">[חבר את מחשבי Windows למסך התכלת](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="b07c6-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b07c6-110">קבל את מזהה סביבת העבודה ואת המפתח הראשי של סביבת העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="b07c6-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b07c6-111">אשף ההתקנה זקוק למידע זה כדי לקבוע את תצורת הסוכן כראוי וכדי להבטיח שהוא יוכל לקיים תקשורת עם צג התכלת.</span><span class="sxs-lookup"><span data-stu-id="b07c6-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="b07c6-112">[דחיפת נתוני אבחון לסביבת העבודה שלך](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="b07c6-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b07c6-113">באפשרותך לדחוף נתוני אבחון מדייר WVD לניתוח יומן הרישום עבור סביבת העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="b07c6-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="b07c6-114">[זיהוי ואבחון של בעיות](https://go.microsoft.com/fwlink/?linkid=2128338) פנימיות או חיצוניות ביחס לWVD.</span><span class="sxs-lookup"><span data-stu-id="b07c6-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b07c6-115">לקבלת מידע נוסף אודות קביעת התצורה של כלי אבחון השירות עבור WVD, ראה [שימוש בניתוח יומני רישום עבור התכונה ' אבחון](https://go.microsoft.com/fwlink/?linkid=2128084)'.</span><span class="sxs-lookup"><span data-stu-id="b07c6-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
