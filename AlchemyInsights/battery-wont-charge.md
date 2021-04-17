---
title: הסוללה אינה נטענת
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002952"
- "5654"
ms.openlocfilehash: fab76114044f71d60dbaf812cd2cd0cc75c8169c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820467"
---
# <a name="battery-wont-charge"></a><span data-ttu-id="f3185-102">הסוללה אינה נטענת</span><span class="sxs-lookup"><span data-stu-id="f3185-102">Battery won't charge</span></span>

<span data-ttu-id="f3185-103">ראשית, ודא שהחיבורים מאובטחים.</span><span class="sxs-lookup"><span data-stu-id="f3185-103">First, make sure connections are secure.</span></span> <span data-ttu-id="f3185-104">אנחנו ממליצים להשתמש רק בספק הכוח המקורי של Microsoft או בספק כוח המורשה על ידי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f3185-104">We strongly recommend that you use only the genuine Microsoft or Microsoft-licensed power supply.</span></span>

<span data-ttu-id="f3185-105">שנית, נסה לכבות את Surface והטען במשך 30 דקות לפחות.</span><span class="sxs-lookup"><span data-stu-id="f3185-105">Secondly, try shutting down your Surface and charge for at least 30 minutes.</span></span> <span data-ttu-id="f3185-106">לאחר מכן, הפעל אותו שוב כדי לראות אם הבעיה נפתרה.</span><span class="sxs-lookup"><span data-stu-id="f3185-106">Then turn it back on to see if that fixes the problem.</span></span>

<span data-ttu-id="f3185-107">**מחובר, אך לא טוען**</span><span class="sxs-lookup"><span data-stu-id="f3185-107">**Plugged in, but not charging**</span></span>

<span data-ttu-id="f3185-108">אם סמל הסוללה בשורת המשימות מראה **מחובר, אינו טוען**, משמעות הדבר ש- Surface מזהה את ספק החשמל, אך אינו מטעין את הסוללה.</span><span class="sxs-lookup"><span data-stu-id="f3185-108">If the battery icon on the taskbar shows **Plugged in, not charging**, it means your Surface detects the power supply but it is not charging the battery.</span></span> <span data-ttu-id="f3185-109">ייתכן ש- Surface יכבה כאשר תנתק אותו.</span><span class="sxs-lookup"><span data-stu-id="f3185-109">Your Surface may turn off when you unplug it.</span></span> <span data-ttu-id="f3185-110">נסה זאת:</span><span class="sxs-lookup"><span data-stu-id="f3185-110">Try this:</span></span>

1. <span data-ttu-id="f3185-111">חבר את Surface.</span><span class="sxs-lookup"><span data-stu-id="f3185-111">Plug in your Surface.</span></span>
2. <span data-ttu-id="f3185-112">בחר את תיבת החיפוש בשורת המשימות, הקלד **מנהל ההתקנים**, ולאחר מכן בחר **מנהל ההתקנים** מרשימת התוצאות.</span><span class="sxs-lookup"><span data-stu-id="f3185-112">Select the search box in the taskbar, type **device manager**, and then select **Device Manager** from the list of results.</span></span>
3. <span data-ttu-id="f3185-113">לחץ על החץ שליד קטגוריית **סוללות**.</span><span class="sxs-lookup"><span data-stu-id="f3185-113">Click the arrow next to the **Batteries** category.</span></span>
4. <span data-ttu-id="f3185-114">הקש פעמיים או לחץ פעמיים על **הסוללה של שיטת הבקרה תואמת-ACPI ב- Surface של Microsoft**, בחר **מנהל התקן** ולחץ על **הסר התקנה > אישור**.</span><span class="sxs-lookup"><span data-stu-id="f3185-114">Double-tap or double-click **Microsoft Surface ACPI-Compliant Control Method Battery**, select the **Driver** tab, and click **Uninstall > OK**.</span></span>
5. <span data-ttu-id="f3185-115">בחר את המחשב בחלק העליון של כל הקטגוריות, בחר את תפריט **הפעולה** ולאחר מכן לחץ על **אתר שינויי חומרה**.</span><span class="sxs-lookup"><span data-stu-id="f3185-115">Select the computer at the top of all the categories, select the **Action** menu, and then click **Scan for hardware changes**.</span></span>
6. <span data-ttu-id="f3185-116">השאר את Surface מחובר.</span><span class="sxs-lookup"><span data-stu-id="f3185-116">Leave your Surface plugged in.</span></span>

<span data-ttu-id="f3185-117">לאחר הסרת מנהל ההתקן של הסוללה, התקן את עדכוני Surface ו- Windows.</span><span class="sxs-lookup"><span data-stu-id="f3185-117">After you remove the battery driver, install Surface and Windows updates.</span></span> <span data-ttu-id="f3185-118">לפרטים, ראה [עדכון חומרה של Surface ו- Windows 10](https://support.microsoft.com/help/4023505).</span><span class="sxs-lookup"><span data-stu-id="f3185-118">See [Update Surface firmware and Windows 10](https://support.microsoft.com/help/4023505) for details.</span></span> <span data-ttu-id="f3185-119">בדוק את הסוללה.</span><span class="sxs-lookup"><span data-stu-id="f3185-119">Check your battery.</span></span> <span data-ttu-id="f3185-120">אם אתה עדיין נתקל בבעיות, ראה [בצע כיבוי כפוי של Surface והפעל אותו מחדש](https://support.microsoft.com/help/4036280/surface-force-a-shut-down-and-restart-your-surface).</span><span class="sxs-lookup"><span data-stu-id="f3185-120">If it's still having problems, see [Force a shut down and restart your Surface](https://support.microsoft.com/help/4036280/surface-force-a-shut-down-and-restart-your-surface).</span></span>

<span data-ttu-id="f3185-121">**מידע נוסף לפתרון בעיות**</span><span class="sxs-lookup"><span data-stu-id="f3185-121">**More troubleshooting information**</span></span>

<span data-ttu-id="f3185-122">נורת ה- LED אמורה להיות מופעלת כאשר מחבר ההפעלה מחובר ל- Surface.</span><span class="sxs-lookup"><span data-stu-id="f3185-122">The LED light should be on when your power connector is plugged into your Surface.</span></span> <span data-ttu-id="f3185-123">אם הוא כבוי או מהבהב, ראה [מה לעשות אם ספק הכוח או המטען של Surface אינו פועל](https://support.microsoft.com/help/4484763/surface-fix-issues-with-your-power-supply).</span><span class="sxs-lookup"><span data-stu-id="f3185-123">If it is off, blinking, or flashing white, please check out [What to do if your Surface power supply or charger doesn’t work](https://support.microsoft.com/help/4484763/surface-fix-issues-with-your-power-supply).</span></span> 

<span data-ttu-id="f3185-124">אם אתה נתקל בבעיות עם Surface Book, ודא שהמסך מחובר למקלדת באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="f3185-124">If you're having problems with your Surface Book, make sure the screen is fully attached to the keyboard.</span></span> <span data-ttu-id="f3185-125">אם הוא עדיין לא נטען, הסר את המסך ונקה את המחברים באמצעות מחק של עיפרון.</span><span class="sxs-lookup"><span data-stu-id="f3185-125">If it still won't charge, remove the screen and clean the connectors with a pencil eraser.</span></span> <span data-ttu-id="f3185-126">אולי תרצה גם לנקות את הסיכות שעל החלק הארוך והצר של המטען שאתה מחבר ל- Surface, ולוודא שהסיכות יבשות.</span><span class="sxs-lookup"><span data-stu-id="f3185-126">You may also want to clean the pins on the long, narrow part of the charger that you plug into your Surface, and make sure the pins are dry.</span></span>

<span data-ttu-id="f3185-127">לדרכים נוספות לפתרון בעיות בסוללה, ראה [הסוללה של Surface אינה נטענת או ש- Surface אינו פועל על סוללה](https://support.microsoft.com/help/4023536/surface-surface-battery-wont-charge).</span><span class="sxs-lookup"><span data-stu-id="f3185-127">To see more ways of troubleshooting battery problems, please check out [Surface battery won’t charge or Surface won’t run on battery](https://support.microsoft.com/help/4023536/surface-surface-battery-wont-charge).</span></span>
