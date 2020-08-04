---
title: קביעת תצורה של DLP נקודת קצה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555559"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="3e392-102">קביעת תצורה של DLP נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="3e392-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="3e392-103">DLP של נקודת הקצה של Microsoft מאפשרת לך להרחיב את יכולת ההגנה של DLP ולפקח על מידע רגיש בהתקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3e392-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="3e392-104">לאחר בקרת התקנים לניהול התקנים, באפשרותך ליצור פריטי מדיניות של DLP כדי לאכוף פעולות הגנה על פריטים.</span><span class="sxs-lookup"><span data-stu-id="3e392-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="3e392-105">ניתן להשתמש בסייר הפעילויות כדי לנטר פעילות עבור פריטים רגישים.</span><span class="sxs-lookup"><span data-stu-id="3e392-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="3e392-106">לקבלת מידע נוסף, ראה [התקני הפנימייה בניהול התקנים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="3e392-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="3e392-107">כדי להתחיל בתחילת הפעלת DLP של נקודת קצה:</span><span class="sxs-lookup"><span data-stu-id="3e392-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="3e392-108">ודא שיש לך את הרישוי המתאים של SKU/מנויים.</span><span class="sxs-lookup"><span data-stu-id="3e392-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="3e392-109">לקבלת מידע נוסף, עיין [ברישוי SKU/מנויים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="3e392-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="3e392-110">בדוק את ההרשאות הנדרשות כדי לאפשר ניהול התקנים, לגשת לעמוד העלייה למטוס או להפעיל את ניטור ההתקן.</span><span class="sxs-lookup"><span data-stu-id="3e392-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="3e392-111">לקבלת מידע נוסף, ראה [הרשאות](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="3e392-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="3e392-112">התקנים מנוהלים לניהול התקנים על-ידי ביצוע הליך התקני העלייה למטוס.</span><span class="sxs-lookup"><span data-stu-id="3e392-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="3e392-113">אם חסרה לך האפשרות ' התקן בחירה ' (תצוגה מקדימה) תחת **הגדרות**M365 תאימות, ודא שיש לך את הרשיון וההרשאות המתאימות שאליהן מפנה לעיל.</span><span class="sxs-lookup"><span data-stu-id="3e392-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="3e392-114">לקבלת מידע נוסף, ראה [התקני כרטיס טיסה](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="3e392-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="3e392-115">צור מדיניות DLP כדי להגן על הפריטים הרגישים.</span><span class="sxs-lookup"><span data-stu-id="3e392-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="3e392-116">לקבלת מידע, ראה [תרחישים של מדיניות DLP של נקודות קצה](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="3e392-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="3e392-117">לקבלת מידע נוסף אודות DLP של נקודות הקצה של Microsoft, ראה [לימוד אודות מניעת אובדן נתונים של microsoft 365 של נקודות קצה (תצוגה מקדימה)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="3e392-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>