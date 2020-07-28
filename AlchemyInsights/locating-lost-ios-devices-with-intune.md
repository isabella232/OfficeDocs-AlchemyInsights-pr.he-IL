---
title: איתור התקנים אבודים iOS עם Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439626"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="1a783-102">איתור התקנים אבודים iOS עם Intune</span><span class="sxs-lookup"><span data-stu-id="1a783-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="1a783-103">הפעלת מצב אבוד בהתקן iOS מאפשרת למנהל לנהל הודעה ומספר טלפון של איש קשר המוצגים על מסך הנעילה.</span><span class="sxs-lookup"><span data-stu-id="1a783-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="1a783-104">לאחר שמצב ' אבד ' מופעל, המנהל יכול להשתמש בפעולת ההתקן אתר כדי לזהות את המיקום הפיזי של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="1a783-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="1a783-105">פעולת ההתקן אתר ב-Intune עובדת עם התקני iOS כדי להציג את המיקום של התקן מסוים על המפה.</span><span class="sxs-lookup"><span data-stu-id="1a783-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="1a783-106">שימוש בפעולה זו מחייב את התקן iOS להיות ב:</span><span class="sxs-lookup"><span data-stu-id="1a783-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="1a783-107">מצב פיקוח</span><span class="sxs-lookup"><span data-stu-id="1a783-107">Supervised mode</span></span>
- <span data-ttu-id="1a783-108">מצב אבוד</span><span class="sxs-lookup"><span data-stu-id="1a783-108">Lost mode</span></span>

<span data-ttu-id="1a783-109">לקבלת מידע נוסף, ראה [הפעלת מצב אבוד על ios/ipados התקנים עם Intune](https://docs.microsoft.com/intune/device-lost-mode) [ולאתר אובדן או נגנב Ios/ipados התקנים עם Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="1a783-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="1a783-110">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="1a783-110">**FAQ**</span></span>

<span data-ttu-id="1a783-111">ש: הנפקת פעולה מרוחקת כדי להסיר נתוני חברה מהתקן, וכעת היא תקועה במצב המתנה.</span><span class="sxs-lookup"><span data-stu-id="1a783-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="1a783-112">ת: כדי שפעולה מרוחקת תושלם בהצלחה, ההתקן המיועד חייב להיות מקוון ובריא.</span><span class="sxs-lookup"><span data-stu-id="1a783-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="1a783-113">במצבים הבאים, הפעולה המרוחקת נשארת במצב המתנה למשך 30 יום, או עד שההתקן מכיר את הפקודה:</span><span class="sxs-lookup"><span data-stu-id="1a783-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="1a783-114">כאשר אין להתקן קישוריות</span><span class="sxs-lookup"><span data-stu-id="1a783-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="1a783-115">כאשר ההתקן מאבד את מצב הניהול שלו עם Intune</span><span class="sxs-lookup"><span data-stu-id="1a783-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="1a783-116">אם אתה סבור שהתקן אינו נמצא עוד בבדיקה ושהוא לא יוכל להסיר נתוני חברה, בחר במחק.</span><span class="sxs-lookup"><span data-stu-id="1a783-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="1a783-117">מחיקה מסירה את רשומת ההתקן כך שלא תופיע עוד ברשימת ההתקנים Intune.</span><span class="sxs-lookup"><span data-stu-id="1a783-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="1a783-118">אם ההתקן הופך לפעיל שוב, המשתמש יצטרך לרשום אותו מחדש.</span><span class="sxs-lookup"><span data-stu-id="1a783-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="1a783-119">ש: מדוע פעולות מרוחקות מסוימות אינן זמינות עבורי לשימוש?</span><span class="sxs-lookup"><span data-stu-id="1a783-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="1a783-120">ת: לא כל הפלטפורמות תומכות בכל פעולות ההתקן המרוחק.</span><span class="sxs-lookup"><span data-stu-id="1a783-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="1a783-121">הפעולות המרוחקות הבאות הן ספציפיות לפלטפורמה, ולכן הן זמינות רק עבור הפלטפורמות שצוינו.</span><span class="sxs-lookup"><span data-stu-id="1a783-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="1a783-122">עקיפת נעילת הפעלה (iOS בלבד)</span><span class="sxs-lookup"><span data-stu-id="1a783-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="1a783-123">התחלה חדשה (Windows בלבד)</span><span class="sxs-lookup"><span data-stu-id="1a783-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="1a783-124">מצב אבוד (iOS בלבד)</span><span class="sxs-lookup"><span data-stu-id="1a783-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="1a783-125">אתר התקן (iOS בלבד)</span><span class="sxs-lookup"><span data-stu-id="1a783-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="1a783-126">הפעל מחדש (Windows בלבד)</span><span class="sxs-lookup"><span data-stu-id="1a783-126">Restart (Windows only)</span></span>

<span data-ttu-id="1a783-127">לקבלת פרטים נוספים אודות כל פעולה, ראה [פעולות התקן זמינות](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="1a783-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>