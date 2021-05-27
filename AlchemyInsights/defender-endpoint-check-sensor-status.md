---
title: מצב חיישן בדיקת נקודת קצה של Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676179"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="034ea-102">מצב חיישן בדיקת נקודת קצה של Defender</span><span class="sxs-lookup"><span data-stu-id="034ea-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="034ea-103">האריח **מכשירים עם בעיות** חיישן ממוקם בלוח המחוונים של פעולות אבטחה.</span><span class="sxs-lookup"><span data-stu-id="034ea-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="034ea-104">אריח זה מספק מידע על היכולת של המכשיר הבודד לספק נתוני חיישנים ולקיים תקשורת עם שירות Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="034ea-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="034ea-105">הוא מדווח על מספר המכשירים שדורשים תשומת לב, עוזר לך לזהות מכשירים בעייתיים ולתקן בעיות ידועות.</span><span class="sxs-lookup"><span data-stu-id="034ea-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="034ea-106">שני מחווני מצב באריח מספקים מידע על מספר המכשירים שלא מדווחים כראוי לשירות:</span><span class="sxs-lookup"><span data-stu-id="034ea-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="034ea-107">**קביעת תצורה שגויה** מכשירים שעשויים לדווח חלקית על נתוני חיישן לשירות Defender for Endpoint ועשויים להסתיים בשגיאות תצורה שיש לתקן.</span><span class="sxs-lookup"><span data-stu-id="034ea-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="034ea-108">**לא פעיל** מכשירים שהפסקו לדווח לשירות Defender for Endpoint במשך יותר משבעה ימים בחודש האחרון.</span><span class="sxs-lookup"><span data-stu-id="034ea-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="034ea-109">לחיצה על אחת מהקבוצות מפנה אותך לרשימה מכשירים, המסוננים בהתאם לאפשרויות שלך.</span><span class="sxs-lookup"><span data-stu-id="034ea-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="034ea-110">ברשימה מכשירים, באפשרותך לסנן את רשימת מצב תקינות לפי המצב הבא:</span><span class="sxs-lookup"><span data-stu-id="034ea-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="034ea-111">**פעיל** מכשירים המדווחים באופן פעיל לשירות Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="034ea-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="034ea-112">**קביעת תצורה שגויה** מכשירים שעשויים לדווח חלקית על נתוני חיישן לשירות Defender for Endpoint, אך קיימים שגיאות תצורה שיש לתקן.</span><span class="sxs-lookup"><span data-stu-id="034ea-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="034ea-113">מכשירים שתצורתם שגויה יכולה לכוללים אחד או שילוב של הבעיות הבאות:</span><span class="sxs-lookup"><span data-stu-id="034ea-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="034ea-114">אין נתוני חיישנים - מכשירים הפסיקו לשלוח נתוני חיישנים.</span><span class="sxs-lookup"><span data-stu-id="034ea-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="034ea-115">ניתן להפעיל התראות מוגבלות מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="034ea-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="034ea-116">תקשורת לקויה - היכולת לקיים תקשורת עם המכשיר לקויה.</span><span class="sxs-lookup"><span data-stu-id="034ea-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="034ea-117">ייתכן ששליחה של קבצים לניתוח עמוק, חסימת קבצים, חסימת מכשיר מהרשת ופעולות אחרות הדורשות תקשורת עם המכשיר לא פועלים.</span><span class="sxs-lookup"><span data-stu-id="034ea-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="034ea-118">**לא פעיל** מכשירים שהפסקו לדווח לשירות Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="034ea-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="034ea-119">באפשרותך להוריד את הרשימה כולה בתבנית CSV באמצעות התכונה ייצוא.</span><span class="sxs-lookup"><span data-stu-id="034ea-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="034ea-120">לקבלת מידע נוסף, ראה [בדיקת מצב תקינות חיישן ב- Microsoft Defender עבור נקודת קצה.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="034ea-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="034ea-121">לקבלת מידע נוסף על מה שגרם להתקן להיות לא פעיל או לא מוגדר כהלכה, ראה [תיקון חיישנים](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)לא בריאים ב- Microsoft Defender עבור נקודת קצה .</span><span class="sxs-lookup"><span data-stu-id="034ea-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
