---
title: עזרה בהגדרת תצוגת אור הלילה
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404662"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="41bf3-102">עזרה בהגדרת תצוגת אור הלילה</span><span class="sxs-lookup"><span data-stu-id="41bf3-102">Help with the night light display setting</span></span>

<span data-ttu-id="41bf3-103">לקבלת מידע נוסף על הגדרות התצוגה של שעות הלילה, ראה [הגדרת התצוגה שלך לזמן לילה ב- Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="41bf3-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="41bf3-104">אם אפשרויות אור הלילה מופיעות באפור בהגדרות, בדוק את מנהל התצוגה:</span><span class="sxs-lookup"><span data-stu-id="41bf3-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="41bf3-105">לחץ על תיבת החיפוש בשורת המשימות והקלד **מנהל ההתקנים** ולאחר מכן בחר **מנהל ההתקנים** בתוצאות החיפוש.</span><span class="sxs-lookup"><span data-stu-id="41bf3-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="41bf3-106">הרחב **את מתאמי תצוגה**.</span><span class="sxs-lookup"><span data-stu-id="41bf3-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="41bf3-107">למרבה הצער, תכונת אור הלילה אינה זמינה אם המכשיר שלך משתמש במנהל התקן DisplayLink או במנהל התקן תצוגה בסיסי.</span><span class="sxs-lookup"><span data-stu-id="41bf3-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="41bf3-108">תכונת אור הלילה משתמשת בטכנולוגיית הגרפיקה האחרונה, כך שייתכן שתצטרך לעדכן את מנהל התצוגה:</span><span class="sxs-lookup"><span data-stu-id="41bf3-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="41bf3-109">בדוק אם קיימים עדכונים **על-ידי עבור אל** התחל  >  **הגדרות** עדכון &  >  **אבטחה** Windows  >  **Update בדוק** אם  >  **קיימים עדכונים.**</span><span class="sxs-lookup"><span data-stu-id="41bf3-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="41bf3-110">או</span><span class="sxs-lookup"><span data-stu-id="41bf3-110">OR</span></span>

- <span data-ttu-id="41bf3-111">בקר באתר האינטרנט של התמיכה של יצרן החומרה כדי להוריד ולהתקין באופן ידני את מנהלי ההתקנים העדכניים ביותר של התצוגה.</span><span class="sxs-lookup"><span data-stu-id="41bf3-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="41bf3-112">איפוס אור לילה ברישום</span><span class="sxs-lookup"><span data-stu-id="41bf3-112">Reset night light in the registry</span></span>

<span data-ttu-id="41bf3-113">אם עדכון מנהל התצוגה לא עבד, ייתכן שתצטרך לאפס את אור הלילה ברישום.</span><span class="sxs-lookup"><span data-stu-id="41bf3-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="41bf3-114">**שים לב:** שלב פתרון בעיות זה מומלץ רק עבור משתמשים מתקדמים.</span><span class="sxs-lookup"><span data-stu-id="41bf3-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="41bf3-115">בעיות חמורות עלולות להתרחש אם תשנה את הרישום באופן שגוי.</span><span class="sxs-lookup"><span data-stu-id="41bf3-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="41bf3-116">לקבלת הגנה נוספת, גבה את הרישום לפני שינויו כדי שתוכל לשחזר אותו אם מתרחשות בעיות.</span><span class="sxs-lookup"><span data-stu-id="41bf3-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="41bf3-117">בתיבת החיפוש, הקלד **regedit** ולאחר מכן בחר **עורך הרישום** בתוצאות החיפוש.</span><span class="sxs-lookup"><span data-stu-id="41bf3-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="41bf3-118">עבור אל מפתח הרישום הבא:</span><span class="sxs-lookup"><span data-stu-id="41bf3-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="41bf3-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="41bf3-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="41bf3-120">יצא ולאחר מכן מחק את מפתח המשנה הבא:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="41bf3-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="41bf3-121">יצא ולאחר מכן מחק את מפתח המשנה הבא:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="41bf3-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="41bf3-122">הפעל מחדש את Windows וודא אם האפשרויות של אור הלילה זמינות.</span><span class="sxs-lookup"><span data-stu-id="41bf3-122">Restart Windows and verify if the night light options are available.</span></span>


