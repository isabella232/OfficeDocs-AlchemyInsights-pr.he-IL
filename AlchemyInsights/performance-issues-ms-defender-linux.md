---
title: בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794007"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="d14ab-102">בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux</span><span class="sxs-lookup"><span data-stu-id="d14ab-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="d14ab-103">מאמר זה מנחה אותך לאורך השלבים של זיהוי בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux.</span><span class="sxs-lookup"><span data-stu-id="d14ab-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="d14ab-104">חשוב לוודא תחילה שהבעיה שבה נתקלת נפתרה בגירסה [העדכנית ביותר.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="d14ab-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="d14ab-105">כדי להתחיל את החקירה, ראה [פתרון בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="d14ab-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="d14ab-106">אי-הכללות</span><span class="sxs-lookup"><span data-stu-id="d14ab-106">Exclusions</span></span>

<span data-ttu-id="d14ab-107">אי-הכללות יכולות לעזור לצמצם בעיות ביצועים.</span><span class="sxs-lookup"><span data-stu-id="d14ab-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="d14ab-108">סקור את האי-הכללות שלך לפני שתתחיל כדי שכל סיכון נוסף יהיה ידוע ותועד.</span><span class="sxs-lookup"><span data-stu-id="d14ab-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="d14ab-109">לקבלת מידע נוסף, ראה [קביעת תצורה ואמת של אי-הכללות עבור Microsoft Defender עבור נקודת קצה ב- Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="d14ab-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="d14ab-110">כאשר יש לך קבצים מרובים & לא לכלול אותם, והם כולם באותה נקודת טעינה, ייתכן שיהיה קל יותר לא לכלול את נקודת הטעינה.</span><span class="sxs-lookup"><span data-stu-id="d14ab-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="d14ab-111">החל מהפצה 101.22.80 בפברואר, באפשרותך לא לכלול נקודת טעינה שלמה.</span><span class="sxs-lookup"><span data-stu-id="d14ab-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="d14ab-112">לדוגמה, אם /mnt/backup הוא נקודת טעינה, באפשרותך להוסיף /mnt/backup לרשימת אי-הכלולות על-ידי הפעלת פקודה זו:</span><span class="sxs-lookup"><span data-stu-id="d14ab-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="d14ab-113">**הערה:** הוספת אי-הכללות מגדילה את הסיכון לתוכנות זדוניות שלא זוהו ויש לטפל ותטמיע איתם בדאגות.</span><span class="sxs-lookup"><span data-stu-id="d14ab-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="d14ab-114">זקוק לעזרה?</span><span class="sxs-lookup"><span data-stu-id="d14ab-114">Need Help?</span></span>

<span data-ttu-id="d14ab-115">כדי לסייע לך בדרך היעילה ביותר, אסוף את נתוני האבחון לפני פתיחת מקרה תמיכה.</span><span class="sxs-lookup"><span data-stu-id="d14ab-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
