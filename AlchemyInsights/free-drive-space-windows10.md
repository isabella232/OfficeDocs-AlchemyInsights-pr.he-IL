---
title: פינוי שטח כונן ב-Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036586"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="c7b9a-102">פינוי שטח כונן ב-Windows 10</span><span class="sxs-lookup"><span data-stu-id="c7b9a-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="c7b9a-103">להלן שתי אפשרויות כדי לפנות שטח כונן ב-Windows:</span><span class="sxs-lookup"><span data-stu-id="c7b9a-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="c7b9a-104">פנה שטח כונן ב-Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="c7b9a-105">פנה מקום עבור עדכונים של Windows 10 עם התקן אחסון חיצוני.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="c7b9a-106">אם עדיין יש לך שטח דיסק נמוך לאחר השימוש בניקוי הדיסק, ייתכן שהתיקיה Temp מתעוררת במהירות באמצעות קבצי יישום (. appx) המשמשים את Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="c7b9a-107">כדי לפתור בעיה זו, אפס את החנות, נקה את מטמון החנות ולאחר מכן הפעלת פותר הבעיות של Windows Update.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="c7b9a-108">ודא ש-Microsoft Store סגור לפני שתמשיך בשלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="c7b9a-109">**שלב 1: איפוס Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="c7b9a-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="c7b9a-110">**הערה** פעולה זו מוחקת לצמיתות את נתוני האפליקציה במכשיר, כולל העדפותיך ופרטי הכניסה.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="c7b9a-111">בחר באפשרות **התחל**  >  **הגדרות**  >  **אפליקציות**  >  של **אפליקציות &**.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="c7b9a-112">ברשימת האפליקציות, אתר ובחר חנות Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="c7b9a-113">בחר **אפשרויות מתקדמות**.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="c7b9a-114">גלול מטה ובחר **איפוס** ולאחר מכן **אשר את איפוס**.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="c7b9a-115">**שלב 2: ניקוי מטמון חנות Microsoft**</span><span class="sxs-lookup"><span data-stu-id="c7b9a-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="c7b9a-116">הקש על מקש סמל Windows + R כדי לפתוח את תיבת הדו ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="c7b9a-117">הקלד wsreset.exe **ובחר אישור**.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="c7b9a-118">נפתח חלון שורת פקודה ריקה.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="c7b9a-119">לאחר כ-10 שניות, החלון נסגר והחנות נפתחת באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="c7b9a-120">**שלב 3: אפס את Windows Update**</span><span class="sxs-lookup"><span data-stu-id="c7b9a-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="c7b9a-121">בחר **התחל**  >  עדכון **הגדרות &**  >    >  **פתרון בעיות** אבטחה.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="c7b9a-122">גלול מטה ובחר **Windows Update** מהרשימה ובחר **הפעלת פותר הבעיות**.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="c7b9a-123">אתחל מחדש את המחשב ובדוק אם אתה עדיין נתקל בבעיה.</span><span class="sxs-lookup"><span data-stu-id="c7b9a-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

