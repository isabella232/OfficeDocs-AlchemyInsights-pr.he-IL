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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657930"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="bf08a-102">קביעת תצורה של DLP של נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="bf08a-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="bf08a-103">Microsoft Endpoint DLP מאפשר לך להרחיב את יכולת ההגנה והניטור של DLP למידע רגיש במכשירי Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bf08a-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="bf08a-104">לאחר שהמכשירים מחוברים לניהול מכשירים, ניתן ליצור פריטי מדיניות DLP כדי לאכוף פעולות הגנה על פריטים.</span><span class="sxs-lookup"><span data-stu-id="bf08a-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="bf08a-105">ניתן להשתמש בסייר הפעילות כדי לנטר פעילות עבור פריטים רגישים.</span><span class="sxs-lookup"><span data-stu-id="bf08a-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="bf08a-106">לקבלת מידע נוסף, ראה [צירוף מכשירים לניהול מכשירים](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="bf08a-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="bf08a-107">כדי להתחיל בעבודה עם DLP בנקודת קצה:</span><span class="sxs-lookup"><span data-stu-id="bf08a-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="bf08a-108">ודא שיש לך את רישוי ה- SKU/המנויים המתאימים.</span><span class="sxs-lookup"><span data-stu-id="bf08a-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="bf08a-109">לקבלת מידע נוסף, ראה [רישוי SKU/מנויים](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="bf08a-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="bf08a-110">בדוק את ההרשאות הדרושות כדי להפוך את ניהול המכשירים לזמין, לגשת לדף הצירוף או להפעיל/לכבות ניטור אחר מכשירים.</span><span class="sxs-lookup"><span data-stu-id="bf08a-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="bf08a-111">לקבלת מידע נוסף, ראה [הרשאות](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="bf08a-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="bf08a-112">צרף מכשירים לניהול מכשירים על-ידי ביצוע ההליך לצירוף מכשירים.</span><span class="sxs-lookup"><span data-stu-id="bf08a-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="bf08a-113">לקבלת מידע נוסף, ראה [צירוף מכשירים](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="bf08a-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="bf08a-114">צור פריטי מדיניות DLP כדי להגן על פריטים רגישים.</span><span class="sxs-lookup"><span data-stu-id="bf08a-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="bf08a-115">לקבלת מידע, ראה [תרחישי מדיניות DLP של נקודת קצה](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="bf08a-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="bf08a-116">לקבלת מידע נוסף על DLP בנקודת הקצה של Microsoft, ראה [קבל מידע נוסף על מניעת אובדן נתונים (תצוגה מקדימה) של נקודת קצה של Microsoft 365](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="bf08a-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="bf08a-117">**שלבי איסוף נתונים חשובים, אם יש צורך בתמיכה:**</span><span class="sxs-lookup"><span data-stu-id="bf08a-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="bf08a-118">הורד [את MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="bf08a-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="bf08a-119">הפעל את הכלי כמנהל מערכת מחלון ה- cmd:</span><span class="sxs-lookup"><span data-stu-id="bf08a-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="bf08a-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="bf08a-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="bf08a-121">כאשר תתבקש לעשות **זאת באמצעות הזן את מספר הדקות לאיסוף מעקבים:**, הזן את מספר הדקות הדרוש כדי להפעיל את התרחיש.</span><span class="sxs-lookup"><span data-stu-id="bf08a-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="bf08a-122">הפעל את התרחיש.</span><span class="sxs-lookup"><span data-stu-id="bf08a-122">Run the scenario.</span></span>

<span data-ttu-id="bf08a-123">אסוף את פלט קובץ ה- Zip כדי להעניק לסוכן התמיכה.</span><span class="sxs-lookup"><span data-stu-id="bf08a-123">Collect the Zip file output to give to the Support agent.</span></span>
