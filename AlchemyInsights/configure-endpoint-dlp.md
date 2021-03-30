---
title: קביעת תצורה של DLP של נקודת קצה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402425"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="66cad-102">קביעת תצורה של DLP של נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="66cad-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="66cad-103">Microsoft Endpoint DLP מאפשר לך להרחיב את יכולת ההגנה והניטור של DLP למידע רגיש במכשירי Windows 10.</span><span class="sxs-lookup"><span data-stu-id="66cad-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="66cad-104">לאחר שהמכשירים מחוברים לניהול מכשירים, ניתן ליצור פריטי מדיניות DLP כדי לאכוף פעולות הגנה על פריטים.</span><span class="sxs-lookup"><span data-stu-id="66cad-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="66cad-105">ניתן להשתמש בסייר הפעילות כדי לנטר פעילות עבור פריטים רגישים.</span><span class="sxs-lookup"><span data-stu-id="66cad-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="66cad-106">לקבלת מידע נוסף, ראה [צירוף מכשירים לניהול מכשירים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="66cad-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="66cad-107">כדי להתחיל בעבודה עם DLP בנקודת קצה:</span><span class="sxs-lookup"><span data-stu-id="66cad-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="66cad-108">ודא שיש לך את רישוי ה- SKU/המנויים המתאימים.</span><span class="sxs-lookup"><span data-stu-id="66cad-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="66cad-109">לקבלת מידע נוסף, ראה [רישוי SKU/מנויים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="66cad-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="66cad-110">בדוק את ההרשאות הדרושות כדי להפוך את ניהול המכשירים לזמין, לגשת לדף הצירוף או להפעיל/לכבות ניטור אחר מכשירים.</span><span class="sxs-lookup"><span data-stu-id="66cad-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="66cad-111">לקבלת מידע נוסף, ראה [הרשאות](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="66cad-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="66cad-112">צרף מכשירים לניהול מכשירים על-ידי ביצוע ההליך לצירוף מכשירים.</span><span class="sxs-lookup"><span data-stu-id="66cad-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="66cad-113">אם האפשרות 'צירוף מכשיר (תצוגה מקדימה)' חסרה לך ב **הגדרות** תאימות M365, אשר שיש לך את הרשיון וההרשאות המתאימים שאליהם מתייחסת ההפניה לעיל.</span><span class="sxs-lookup"><span data-stu-id="66cad-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="66cad-114">לקבלת מידע נוסף, ראה [צירוף מכשירים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="66cad-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="66cad-115">צור פריטי מדיניות DLP כדי להגן על פריטים רגישים.</span><span class="sxs-lookup"><span data-stu-id="66cad-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="66cad-116">לקבלת מידע, ראה [תרחישי מדיניות DLP של נקודת קצה](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="66cad-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="66cad-117">לקבלת מידע נוסף על DLP בנקודת הקצה של Microsoft, ראה [קבל מידע נוסף על מניעת אובדן נתונים (תצוגה מקדימה) של נקודת קצה של Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="66cad-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="66cad-118">**שלבי איסוף נתונים חשובים, אם יש צורך בתמיכה:**</span><span class="sxs-lookup"><span data-stu-id="66cad-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="66cad-119">הורד תצוגה מקדימה של MDATP Client Analyzer מ- [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="66cad-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="66cad-120">הפעל את הכלי כמנהל מערכת מחלון ה- cmd:</span><span class="sxs-lookup"><span data-stu-id="66cad-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="66cad-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="66cad-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="66cad-122">כאשר תופיעה הבקשה "הקלד את מספר הדקות לאיסוף מעקבים: ", הזן את מספר הדקות הדרושות כדי להפעיל את התרחיש</span><span class="sxs-lookup"><span data-stu-id="66cad-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="66cad-123">הפעל את התרחיש</span><span class="sxs-lookup"><span data-stu-id="66cad-123">Run the scenario</span></span>

<span data-ttu-id="66cad-124">אסוף את פלט קובץ ה- Zip שיינתן לסוכן התמיכה.</span><span class="sxs-lookup"><span data-stu-id="66cad-124">Collect the Zip file output to be given to the Support agent.</span></span>
