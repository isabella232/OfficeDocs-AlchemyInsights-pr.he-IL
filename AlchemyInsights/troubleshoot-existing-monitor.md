---
title: פתרון בעיות בצג הקיים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738570"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="94d28-102">פתרון בעיות בצג קיים</span><span class="sxs-lookup"><span data-stu-id="94d28-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="94d28-103">נסה את הפתרונות הבאים כדי לפתור בעיות בצג.</span><span class="sxs-lookup"><span data-stu-id="94d28-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="94d28-104">**רענן את תצוגת הצג:**</span><span class="sxs-lookup"><span data-stu-id="94d28-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="94d28-105">לחץ על המקשים הבאים בו: מקש Windows + Ctrl + Shift + B. פעולה זו תרענן את התקשורת עם מנהל ההתקן הגרפי.</span><span class="sxs-lookup"><span data-stu-id="94d28-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="94d28-106">הצגים שלכם ימצמץ ברגע. ויחזרו אחרי כמה שניות</span><span class="sxs-lookup"><span data-stu-id="94d28-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="94d28-107">**פתרון בעיות בחומרת הצג:**</span><span class="sxs-lookup"><span data-stu-id="94d28-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="94d28-108">נתק את הכבל המחבר את המחשב לצג וחבר אותו חזרה.</span><span class="sxs-lookup"><span data-stu-id="94d28-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="94d28-109">נתק כל התקן שאינו חיוני מהמחשב (כגון מתאמים או רציפים).</span><span class="sxs-lookup"><span data-stu-id="94d28-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="94d28-110">**אם התקנת לאחרונה עדכון במחשב שלך, באפשרותך להחזיר את מנהל ההתקן של התצוגה:**</span><span class="sxs-lookup"><span data-stu-id="94d28-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="94d28-111">בחר באפשרות **התחל**, הקלד **מנהל ההתקנים**ובחר **במנהל ההתקנים** מהתוצאות.</span><span class="sxs-lookup"><span data-stu-id="94d28-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="94d28-112">הרחב את המקטע **מתאמי תצוגה** , לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה שלך ובחר **מאפיינים**.</span><span class="sxs-lookup"><span data-stu-id="94d28-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="94d28-113">נווט אל הכרטיסיה **מנהל התקן** ובחר באפשרות ' **חזור על התקן קודם**'.</span><span class="sxs-lookup"><span data-stu-id="94d28-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="94d28-114">הערה: אם אפשרות זו אינה זמינה או מעומעמת, בחר באפשרות **לא** מתוך האפשרויות שלהלן כדי לעבור לשלב הבא.</span><span class="sxs-lookup"><span data-stu-id="94d28-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="94d28-115">ייתכן שיהיה עליך להפעיל מחדש את המחשב לפני שהשינויים ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="94d28-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="94d28-116">**הסר והתקן מחדש את מנהל ההתקן של התצוגה:**</span><span class="sxs-lookup"><span data-stu-id="94d28-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="94d28-117">בחר באפשרות **התחל**, הקלד **מנהל ההתקנים**ובחר **במנהל ההתקנים** מהתוצאות.</span><span class="sxs-lookup"><span data-stu-id="94d28-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="94d28-118">הרחב את המקטע **מתאמי תצוגה** , לחץ באמצעות לחצן העכבר הימני על מתאם התצוגה שלך ובחר באפשרות **הסר התקנה**</span><span class="sxs-lookup"><span data-stu-id="94d28-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="94d28-119">בחר את התיבה הסמוכה כדי **למחוק את תוכנת מנהל ההתקן עבור התקן זה** ובחר **בהסרת התקנה**.</span><span class="sxs-lookup"><span data-stu-id="94d28-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="94d28-120">הערה: ייתכן שתתבקש להפעיל מחדש את המחשב בשלב זה.</span><span class="sxs-lookup"><span data-stu-id="94d28-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="94d28-121">הקפד לרשום את ההוראות הנותרות לפני שתפעיל מחדש.</span><span class="sxs-lookup"><span data-stu-id="94d28-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="94d28-122">פתח שוב את מנהל ההתקנים.</span><span class="sxs-lookup"><span data-stu-id="94d28-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="94d28-123">הרחב את המקטע **מתאמי תצוגה** , לחץ לחיצה ימנית על מתאם התצוגה שלך ובחר באפשרות **עדכן מנהל התקן**.</span><span class="sxs-lookup"><span data-stu-id="94d28-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="94d28-124">בחר **באפשרות חיפוש באופן אוטומטי עבור תוכנת מנהל התקן של עדכון** ופעל לפי הוראות ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="94d28-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>