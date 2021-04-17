---
title: פתרון בעיות בצג קיים
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824580"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="07828-102">פתרון בעיות בצג קיים</span><span class="sxs-lookup"><span data-stu-id="07828-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="07828-103">נסה פתרונות אלה כדי לפתור בעיות בצג.</span><span class="sxs-lookup"><span data-stu-id="07828-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="07828-104">**רענן את תצוגת הצג:**</span><span class="sxs-lookup"><span data-stu-id="07828-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="07828-105">הקש על המקשים הבאים בו-זמנית: מקש Windows + Ctrl + Shift + B. פעולה זו תרענן את התקשורת עם מנהל ההתקן של הגרפיקה.</span><span class="sxs-lookup"><span data-stu-id="07828-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="07828-106">הצגים שלך יהבהבו לרגע ותחזור לאחר כמה שניות.</span><span class="sxs-lookup"><span data-stu-id="07828-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="07828-107">**פתרון בעיות בחומרת צג:**</span><span class="sxs-lookup"><span data-stu-id="07828-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="07828-108">נתק את הכבל המחבר את המחשב לצג וחבר אותו בחזרה.</span><span class="sxs-lookup"><span data-stu-id="07828-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="07828-109">נתק מכשירים שאינם חיוניים מהמחשב שלך (כגון מתאמים או תחנות עגינה).</span><span class="sxs-lookup"><span data-stu-id="07828-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="07828-110">**אם התקנת לאחרונה עדכון במחשב, באפשרותך להחזיר את מנהל התצוגה:**</span><span class="sxs-lookup"><span data-stu-id="07828-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="07828-111">בחר **התחל**, הקלד **מנהל ההתקנים** ובחר **מנהל ההתקנים** מתוך התוצאות.</span><span class="sxs-lookup"><span data-stu-id="07828-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="07828-112">הרחב את **המקטע מתאמי** תצוגה, לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה ובחר **מאפיינים**.</span><span class="sxs-lookup"><span data-stu-id="07828-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="07828-113">נווט אל הכרטיסיה **מנהל** התקן ובחר חזור **למנהל התקן.**</span><span class="sxs-lookup"><span data-stu-id="07828-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="07828-114">הערה: אם אפשרות זו אינה זמינה או אם היא מופיעה באפור, בחר **לא** מהאפשרויות שלהלן כדי לעבור לשלב הבא.</span><span class="sxs-lookup"><span data-stu-id="07828-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="07828-115">ייתכן שיהיה עליך להפעיל מחדש את המחשב לפני ששינויים אלה ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="07828-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="07828-116">**הסר את התקנת מנהל התצוגה והתקן אותו מחדש:**</span><span class="sxs-lookup"><span data-stu-id="07828-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="07828-117">בחר **התחל**, הקלד **מנהל ההתקנים** ובחר **מנהל ההתקנים** מתוך התוצאות.</span><span class="sxs-lookup"><span data-stu-id="07828-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="07828-118">הרחב את **המקטע מתאמי תצוגה,** לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה ובחר הסר **התקנה של מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="07828-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="07828-119">בחר את התיבה לצד מחק **את תוכנת מנהל ההתקן עבור מכשיר זה ובחר** הסר **התקנה**.</span><span class="sxs-lookup"><span data-stu-id="07828-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="07828-120">הערה: ייתכן שתתבקש להפעיל מחדש את המחשב בשלב זה.</span><span class="sxs-lookup"><span data-stu-id="07828-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="07828-121">הקפד לרשום את ההוראות הנותרות לפני ההפעלה מחדש.</span><span class="sxs-lookup"><span data-stu-id="07828-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="07828-122">פתח שוב את מנהל ההתקנים.</span><span class="sxs-lookup"><span data-stu-id="07828-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="07828-123">הרחב את **המקטע מתאמי תצוגה,** לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה ובחר **עדכן מנהל התקן**.</span><span class="sxs-lookup"><span data-stu-id="07828-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="07828-124">בחר **חפש באופן אוטומטי את תוכנת מנהל ההתקן של העדכון** ובצע את הוראות ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="07828-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>