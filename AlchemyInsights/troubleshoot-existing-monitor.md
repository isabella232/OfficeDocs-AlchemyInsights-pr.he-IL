---
title: פתרון בעיות בצג קיים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690712"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="cfca5-102">פתרון בעיות בצג קיים</span><span class="sxs-lookup"><span data-stu-id="cfca5-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="cfca5-103">נסה פתרונות אלה כדי לפתור בעיות בצג.</span><span class="sxs-lookup"><span data-stu-id="cfca5-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="cfca5-104">**רענן את תצוגת הצג:**</span><span class="sxs-lookup"><span data-stu-id="cfca5-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="cfca5-105">הקש על המקשים הבאים בו: מקש Windows + Ctrl + Shift + B. פעולה זו תרענן תקשורת עם מנהל הגרפיקה.</span><span class="sxs-lookup"><span data-stu-id="cfca5-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="cfca5-106">הצגים יהבהבו במהירות ויחזרו לאחר כמה שניות.</span><span class="sxs-lookup"><span data-stu-id="cfca5-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="cfca5-107">**פתרון בעיות בחומרה של צג:**</span><span class="sxs-lookup"><span data-stu-id="cfca5-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="cfca5-108">נתק את הכבל המחבר את המחשב לצג וחבר אותו שוב.</span><span class="sxs-lookup"><span data-stu-id="cfca5-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="cfca5-109">נתק מכשירים שאינם חיוניים מהמחשב שלך (כגון מתאמים או רציפים).</span><span class="sxs-lookup"><span data-stu-id="cfca5-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="cfca5-110">**אם התקנת עדכון במחשב שלך לאחרונה, באפשרותך להחזיר את מנהל ההתקן של התצוגה:**</span><span class="sxs-lookup"><span data-stu-id="cfca5-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="cfca5-111">בחר **התחל**, הקלד **מנהל התקנים**ובחר **מנהל ההתקנים** מהתוצאות.</span><span class="sxs-lookup"><span data-stu-id="cfca5-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="cfca5-112">הרחב את המקטע **מתאמי תצוגה** , לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה, ידיים ובחר **מאפיינים**.</span><span class="sxs-lookup"><span data-stu-id="cfca5-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="cfca5-113">נווט אל הכרטיסיה **מנהל התקן** ובחר באפשרות **חזור למנהל התקן קודם**.</span><span class="sxs-lookup"><span data-stu-id="cfca5-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="cfca5-114">הערה: אם אפשרות זו אינה זמינה או שהיא מעומעמת, בחר **לא** מתוך האפשרויות הבאות כדי לעבור לשלב הבא.</span><span class="sxs-lookup"><span data-stu-id="cfca5-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="cfca5-115">ייתכן שתצטרך להפעיל מחדש את המחשב לפני ששינויים אלה ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="cfca5-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="cfca5-116">**הסר את ההתקנה והתקן מחדש את מנהל התצוגה:**</span><span class="sxs-lookup"><span data-stu-id="cfca5-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="cfca5-117">בחר **התחל**, הקלד **מנהל התקנים**ובחר **מנהל ההתקנים** מהתוצאות.</span><span class="sxs-lookup"><span data-stu-id="cfca5-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="cfca5-118">הרחב את המקטע ' **מתאמי תצוגה** ', לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה, ידיים ובחר **התקן**</span><span class="sxs-lookup"><span data-stu-id="cfca5-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="cfca5-119">בחר את התיבה לצד **מחק את תוכנת מנהל ההתקן עבור התקן זה ובחר** **הסר התקנה**.</span><span class="sxs-lookup"><span data-stu-id="cfca5-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="cfca5-120">הערה: ייתכן שתתבקש להפעיל מחדש את המחשב בשלב זה.</span><span class="sxs-lookup"><span data-stu-id="cfca5-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="cfca5-121">הקפד לרשום את ההוראות הנותרות לפני ההפעלה מחדש.</span><span class="sxs-lookup"><span data-stu-id="cfca5-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="cfca5-122">פתח שוב את מנהל ההתקנים.</span><span class="sxs-lookup"><span data-stu-id="cfca5-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="cfca5-123">הרחב את המקטע ' **מתאמי תצוגה** ', לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה ובחר **עדכן מנהל התקן**.</span><span class="sxs-lookup"><span data-stu-id="cfca5-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="cfca5-124">בחר **חפש באופן אוטומטי את תוכנת מנהל ההתקן** ובצע את הוראות ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="cfca5-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>