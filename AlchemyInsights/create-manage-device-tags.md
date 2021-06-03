---
title: יצירה וניהול של תגיות או קבוצות של מכשירים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731665"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="c288a-102">יצירה וניהול של תגיות או קבוצות של מכשירים</span><span class="sxs-lookup"><span data-stu-id="c288a-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="c288a-103">הוסף תגיות במכשירים כדי ליצור קשר לקבוצה לוגית.</span><span class="sxs-lookup"><span data-stu-id="c288a-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="c288a-104">תגיות מכשיר תומכות במיפוי תקין של הרשת, ומאפשרות לך לצרף תגיות שונות כדי ללכוד הקשר ולאפשר יצירת רשימה דינאמית כחלק מתקרית.</span><span class="sxs-lookup"><span data-stu-id="c288a-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="c288a-105">ניתן להשתמש תגיות כמסנן בתצוגת רשימת מכשירים או כדי לקבץ מכשירים.</span><span class="sxs-lookup"><span data-stu-id="c288a-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="c288a-106">לקבלת מידע נוסף אודות קיבוץ מכשירים, [ראה יצירה וניהול של תגיות מכשיר](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="c288a-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="c288a-107">באפשרותך להוסיף תגיות במכשירים על-ידי:</span><span class="sxs-lookup"><span data-stu-id="c288a-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="c288a-108">שימוש בפורטל</span><span class="sxs-lookup"><span data-stu-id="c288a-108">Using the portal</span></span>

- <span data-ttu-id="c288a-109">הגדרת ערך מפתח רישום</span><span class="sxs-lookup"><span data-stu-id="c288a-109">Setting a registry key value</span></span>
 
<span data-ttu-id="c288a-110">**הערה:** ייתכן שיש השהיה בין הזמן שבו תגית נוספת למכשיר לבין הזמינות שלו ברשימת המכשירים ובדף המכשיר.</span><span class="sxs-lookup"><span data-stu-id="c288a-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="c288a-111">כדי להוסיף תגיות מכשיר באמצעות API, ראה [הוספה או הסרה של API של תגיות מכשיר](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="c288a-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="c288a-112">הוספה וניהול של תגיות מכשיר באמצעות הפורטל</span><span class="sxs-lookup"><span data-stu-id="c288a-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="c288a-113">בחר את המכשיר שבו ברצונך לנהל תגיות.</span><span class="sxs-lookup"><span data-stu-id="c288a-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="c288a-114">באפשרותך לבחור או לחפש מכשיר מכל אחת מהתצוגות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c288a-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="c288a-115">**לוח מחוונים של פעולות אבטחה** בחר את שם המכשיר מתוך המקטע מכשירים מובילים עם התראות פעילות.</span><span class="sxs-lookup"><span data-stu-id="c288a-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="c288a-116">**תור התראות** - בחר את שם המכשיר לצד סמל המכשיר מתור ההתראות.</span><span class="sxs-lookup"><span data-stu-id="c288a-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="c288a-117">**רשימת** מכשירים - בחר את שם המכשיר מרשימת המכשירים.</span><span class="sxs-lookup"><span data-stu-id="c288a-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="c288a-118">**תיבת חיפוש** - בחר התקן מהתפריט הנפתח והזן את שם המכשיר.</span><span class="sxs-lookup"><span data-stu-id="c288a-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="c288a-119">באפשרותך גם להגיע לדף ההתראה דרך תצוגות הקובץ וה- IP.</span><span class="sxs-lookup"><span data-stu-id="c288a-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="c288a-120">בחר **נהל תגיות** משורת פעולות תגובה.</span><span class="sxs-lookup"><span data-stu-id="c288a-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="c288a-121">הקלד כדי לחפש או ליצור תגיות.</span><span class="sxs-lookup"><span data-stu-id="c288a-121">Type to find or create tags.</span></span>

<span data-ttu-id="c288a-122">תגיות מתווספות אל תצוגת המכשיר ומשתקפות בתצוגת הרשימה מכשירים.</span><span class="sxs-lookup"><span data-stu-id="c288a-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="c288a-123">לאחר מכן תוכל להשתמש במסנן תגיות כדי לראות את רשימת המכשירים הרלוונטית.</span><span class="sxs-lookup"><span data-stu-id="c288a-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="c288a-124">לקבלת מידע נוסף, ראה [יצירה וניהול של תגיות מכשיר](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="c288a-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>