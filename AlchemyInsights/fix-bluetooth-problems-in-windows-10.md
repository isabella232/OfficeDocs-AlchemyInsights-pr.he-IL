---
title: תקן בעיות Bluetooth ב-Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268634"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="f823f-102">תקן בעיות Bluetooth ב-Windows 10</span><span class="sxs-lookup"><span data-stu-id="f823f-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="f823f-103">אם הסמל של Bluetooth חסר או שאין אפשרות להפעיל או לבטל את Bluetooth, ייתכן שתרצה להפעיל את פותר בעיות ה-Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="f823f-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="f823f-104">[פתח את הגדרות פתרון בעיות](ms-settings:troubleshoot), לחץ על **Bluetooth** תחת **חיפוש ותיקון בעיות אחרות**, לחץ על **הפעל את פותר הבעיות**.</span><span class="sxs-lookup"><span data-stu-id="f823f-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="f823f-105">אם אינך רואה את סמל ה-Bluetooth, אך Bluetooth מופיע במנהל ההתקנים:</span><span class="sxs-lookup"><span data-stu-id="f823f-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="f823f-106">במנהל ההתקנים, לחץ על **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="f823f-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="f823f-107">לחץ והחזק (או לחץ לחיצה ימנית) על שם מתאם ה-Bluetooth ולחץ על **הסר התקן**.</span><span class="sxs-lookup"><span data-stu-id="f823f-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="f823f-108">כבה את התקן Windows, המתן מספר שניות ולאחר מכן הפעל אותו בחזרה.</span><span class="sxs-lookup"><span data-stu-id="f823f-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="f823f-109">Windows ינסה להתקין מחדש את מנהל ההתקן.</span><span class="sxs-lookup"><span data-stu-id="f823f-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="f823f-110">אם התקנת לאחרונה עדכונים של Windows 10 או שודרגו ל-Windows 10, ייתכן שתרצה לבדוק אם קיימים עדכוני מנהלי התקנים:</span><span class="sxs-lookup"><span data-stu-id="f823f-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="f823f-111">במנהל ההתקנים, לחץ על **Bluetooth**ולאחר מכן לחץ על שם מתאם ה-bluetooth (שעשוי לכלול את המילה "רדיו").</span><span class="sxs-lookup"><span data-stu-id="f823f-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="f823f-112">לחץ והחזק (או לחץ לחיצה ימנית) על מתאם Bluetooth ולאחר מכן לחץ על > עדכן**חיפוש במנהל התקן באופן אוטומטי עבור תוכנת מנהל התקן מעודכנת**. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="f823f-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="f823f-113">בצע את השלבים ולאחר מכן לחץ על **סגור**.</span><span class="sxs-lookup"><span data-stu-id="f823f-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="f823f-114">אם Windows אינו מוצא מנהל התקן Bluetooth חדש, בקר באתר האינטרנט של יצרן המחשב והורד את מנהל ההתקן העדכני ביותר של Bluetooth משם.</span><span class="sxs-lookup"><span data-stu-id="f823f-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="f823f-115">לאחר שהורדת אותו, לחץ על >  **עדכן מנהל התקן** > **עיון במחשב שלי לאיתור תוכנות מנהלי התקנים**עבור המיקום שבו קבצי מנהלי ההתקנים מאוחסנים ב-_ gt_ **OK** > ובצע את השלבים**הבאים**להתקנה.\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="f823f-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="f823f-116">לאחר התקנת מנהל ההתקן המעודכן, הפעל מחדש את המחשב ולאחר מכן בדוק אם הבעיה מתקנת את בעיית החיבור.</span><span class="sxs-lookup"><span data-stu-id="f823f-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="f823f-117">לקבלת פרטים נוספים על פתרון בעיות Bluetooth, עיין במאמר המלא, [תקן בעיות bluetooth ב-Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="f823f-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
