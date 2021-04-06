---
title: פינוי שטח בכונן ב- Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505357"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="4d3b1-102">פינוי שטח בכונן ב- Windows 10</span><span class="sxs-lookup"><span data-stu-id="4d3b1-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="4d3b1-103">להלן שתי אפשרויות לפינוי שטח בכונן ב- Windows:</span><span class="sxs-lookup"><span data-stu-id="4d3b1-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="4d3b1-104">פנה שטח בכונן ב- Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="4d3b1-105">פנה שטח עבור עדכוני Windows 10 באמצעות התקן אחסון חיצוני.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="4d3b1-106">אם עדיין יש לך שטח דיסק מועט לאחר השימוש ב'ניקוי דיסק', ייתכן שתיקיית Temp מתמלאת במהירות בקבצי אפליקציה (appx.) המשמשים את Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="4d3b1-107">כדי לפתור בעיה זו, אפס את ה- Store, נקה את מטמון ה- Store ולאחר מכן הפעל את פותר הבעיות של Windows Update.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="4d3b1-108">ודא ש- Microsoft Store סגורה לפני שתמשיך לביצוע שלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="4d3b1-109">**שלב 1: איפוס Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="4d3b1-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="4d3b1-110">**הערה** פעולה זו תמחק לצמיתות את נתוני האפליקציה במכשיר, כולל ההעדפות ופרטי הכניסה.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="4d3b1-111">בחר **התחל** > **הגדרות** > **אפליקציות** > **אפליקציות ותכונות**.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="4d3b1-112">ברשימת האפליקציות, אתר ובחר את Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="4d3b1-113">בחר **אפשרויות מתקדמות**.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="4d3b1-114">גלול מטה ובחר באפשרות **איפוס** ולאחר מכן **אשר איפוס**.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="4d3b1-115">**שלב 2: ניקוי המטמון של Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="4d3b1-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="4d3b1-116">הקש על מקש סמל Windows + ‏R כדי לפתוח את תיבת הדו-שיח 'הפעלה'.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="4d3b1-117">הקלד wsreset.exe ובחר באפשרות **אישור**.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="4d3b1-118">נפתח חלון ריק של שורת פקודה.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="4d3b1-119">לאחר כ- 10 שניות, החלון ייסגר וה- Store תיפתח באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="4d3b1-120">**שלב 3: איפוס Windows Update**</span><span class="sxs-lookup"><span data-stu-id="4d3b1-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="4d3b1-121">בחר **התחל** > **הגדרות** > **עדכון ואבטחה** > **פתרון בעיות**.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="4d3b1-122">גלול מטה ובחר את **Windows Update** מהרשימה ולאחר מכן בחר באפשרות **הפעל את פותר הבעיות**.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="4d3b1-123">אתחל מחדש את המחשב ובדוק אם אתה עדיין נתקל בבעיה.</span><span class="sxs-lookup"><span data-stu-id="4d3b1-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

