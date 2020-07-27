---
title: עקיפת נעילת ההפעלה על מתחת פיקוח התקנים iOS עם Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423733"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="f22fc-102">עקיפת נעילת ההפעלה על מתחת פיקוח התקנים iOS עם Intune</span><span class="sxs-lookup"><span data-stu-id="f22fc-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="f22fc-103">היכולת לעקוף את נעילת ההפעלה בהתקני iOS מקלה על השחזור מתרחיש שבו משתמש מאפשר נעילת הפעלה בהתקן חברה, ולאחר מכן עוזב את החברה.</span><span class="sxs-lookup"><span data-stu-id="f22fc-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="f22fc-104">דרישות מראש לעקיפת נעילת הפעלה כוללות:</span><span class="sxs-lookup"><span data-stu-id="f22fc-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="f22fc-105">. מכשיר הוא שהוא "מפוקח"</span><span class="sxs-lookup"><span data-stu-id="f22fc-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="f22fc-106">נעילת ההפעלה מופעלת בהצלחה באמצעות מדיניות הגבלת התקן iOS ב-Intune.</span><span class="sxs-lookup"><span data-stu-id="f22fc-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="f22fc-107">בנוסף, בעת עקיפת נעילת הפעלה, עליך:</span><span class="sxs-lookup"><span data-stu-id="f22fc-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="f22fc-108">. מחזיק את המכשיר נקי מבחינה פיזית</span><span class="sxs-lookup"><span data-stu-id="f22fc-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="f22fc-109">העתק את הקוד לפני שאתה מנפיק את המחיקה.</span><span class="sxs-lookup"><span data-stu-id="f22fc-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="f22fc-110">**הערה:** קוד המחיקה אינו תלוי רישיות, כך שהתווים "-" אינם נדרשים.</span><span class="sxs-lookup"><span data-stu-id="f22fc-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="f22fc-111">לקבלת פרטים, ראה [עקיפת נעילת הפעלה על התקני iOS בפיקוח עם Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="f22fc-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="f22fc-112">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="f22fc-112">**FAQ**</span></span>

<span data-ttu-id="f22fc-113">ש: **הנפקת פעולה מרוחקת כדי להסיר נתוני חברה מהתקן, וכעת היא תקועה במצב המתנה.**</span><span class="sxs-lookup"><span data-stu-id="f22fc-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="f22fc-114">ת: כדי שפעולה מרוחקת תושלם בהצלחה, ההתקן המיועד חייב להיות מקוון ובריא.</span><span class="sxs-lookup"><span data-stu-id="f22fc-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="f22fc-115">במצבים הבאים, הפעולה המרוחקת נשארת במצב המתנה למשך 30 יום, או עד שההתקן מכיר בפקודה כאשר ההתקן:</span><span class="sxs-lookup"><span data-stu-id="f22fc-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="f22fc-116">אין קישוריות.</span><span class="sxs-lookup"><span data-stu-id="f22fc-116">Does not have connectivity.</span></span>
- <span data-ttu-id="f22fc-117">מאבד את מצבו הניהולי. עם Intune</span><span class="sxs-lookup"><span data-stu-id="f22fc-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="f22fc-118">אם אתה סבור שהתקן אינו נמצא עוד בבדיקה ושהוא לא יסיר נתוני חברה, בחר במחק.</span><span class="sxs-lookup"><span data-stu-id="f22fc-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="f22fc-119">מחיקה מסירה את רשומת ההתקן כך שלא תופיע עוד ברשימת ההתקנים Intune.</span><span class="sxs-lookup"><span data-stu-id="f22fc-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="f22fc-120">כדי שההתקן יהפוך לפעיל שוב, על המשתמש שלו לרשום מחדש את ההתקן.</span><span class="sxs-lookup"><span data-stu-id="f22fc-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="f22fc-121">ש: **מדוע פעולות מרוחקות מסוימות אינן זמינות עבורי לשימוש?**</span><span class="sxs-lookup"><span data-stu-id="f22fc-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="f22fc-122">ת: לא כל הפלטפורמות תומכות בכל פעולות ההתקן המרוחק.</span><span class="sxs-lookup"><span data-stu-id="f22fc-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="f22fc-123">הפעולות המרוחקות הבאות הן ספציפיות לפלטפורמה.</span><span class="sxs-lookup"><span data-stu-id="f22fc-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="f22fc-124">עקיפת נעילת הפעלה (iOS בלבד)</span><span class="sxs-lookup"><span data-stu-id="f22fc-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="f22fc-125">התחלה חדשה (Windows בלבד)</span><span class="sxs-lookup"><span data-stu-id="f22fc-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="f22fc-126">מצב אבוד (iOS בלבד)</span><span class="sxs-lookup"><span data-stu-id="f22fc-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="f22fc-127">אתר התקן (iOS בלבד)</span><span class="sxs-lookup"><span data-stu-id="f22fc-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="f22fc-128">הפעל מחדש (Windows בלבד)</span><span class="sxs-lookup"><span data-stu-id="f22fc-128">Restart (Windows only)</span></span>

<span data-ttu-id="f22fc-129">לקבלת פרטים נוספים אודות כל פעולה, ראה [פעולות התקן זמינות](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="f22fc-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>