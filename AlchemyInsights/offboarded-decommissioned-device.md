---
title: בעיות בהסרת מכשיר לא מחובר או הוצא ממכשיר המלאי של המכשיר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564338"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="e85e2-102">בעיות בהסרת מכשיר לא מחובר או הוצא ממכשיר המלאי של המכשיר</span><span class="sxs-lookup"><span data-stu-id="e85e2-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="e85e2-103">Microsoft Defender עבור נקודת קצה אינו מאפשר כעת הסרה ידנית של רשומת המכשיר של מכשיר לא מחובר או הוצא מהמכשיר מהמלאי של המכשיר.</span><span class="sxs-lookup"><span data-stu-id="e85e2-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="e85e2-104">למטרות אבטחה, המכשיר נשאר בפורטל כהקלטה היסטורית של עד 180 יום.</span><span class="sxs-lookup"><span data-stu-id="e85e2-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="e85e2-105">עם זאת, נתוני המכשיר מטוהרים בהתאם לתקופת השמירה שתצורתה נקבעה.</span><span class="sxs-lookup"><span data-stu-id="e85e2-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="e85e2-106">**הערה:** התקן מחוץ ל- offboarded או offcommissioned עובר באופן אוטומטי למצב **לא** פעיל לאחר שבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="e85e2-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="e85e2-107">בנוסף, מכשירים אינם פעילים ב- 30 הימים האחרונים אינם גורמים לנתונים המשקפים את הארגון שלך Threat and Vulnerability Management חשיפה או ניקוד מאובטח של Microsoft עבור מכשירים.</span><span class="sxs-lookup"><span data-stu-id="e85e2-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="e85e2-108">אם עדיין אינך מעוניין לראות מכשירים מסוימים בתצוגת מלאי מכשירים, נסה למקם תגית מכשיר כדי לסנן את המכשיר שהופסק מהתיבה מלאי מכשיר.</span><span class="sxs-lookup"><span data-stu-id="e85e2-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="e85e2-109">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="e85e2-109">For more information, see:</span></span>

[<span data-ttu-id="e85e2-110">מכשירים לא זמינים בשירות Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="e85e2-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="e85e2-111">ציון חשיפה Threat and Vulnerability Management</span><span class="sxs-lookup"><span data-stu-id="e85e2-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="e85e2-112">תיקון חיישנים לא בריאים ב- Microsoft Defender עבור נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="e85e2-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="e85e2-113">כיצד להשתמש בתיוג ביעילות (חלק 1)</span><span class="sxs-lookup"><span data-stu-id="e85e2-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="e85e2-114">כיצד להשתמש בתיוג ביעילות (חלק 2)</span><span class="sxs-lookup"><span data-stu-id="e85e2-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="e85e2-115">כיצד להשתמש בתיוג ביעילות (חלק 3)</span><span class="sxs-lookup"><span data-stu-id="e85e2-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




