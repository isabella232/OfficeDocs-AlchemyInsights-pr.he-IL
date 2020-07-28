---
title: הסרת נתונים וניגוב התקנים מIntune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439649"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="dc2e5-102">הסרת נתונים וניגוב התקנים מIntune</span><span class="sxs-lookup"><span data-stu-id="dc2e5-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="dc2e5-103">ניתן להשתמש בפעולות מרוחקות של התקן פרישה ומחיקה של התקן כדי להסיר נתוני חברה המנוהלים על-ידי Intune או לבצע איפוס של המפעל ולהחזיר את ההתקן להגדרות ברירת המחדל שלו.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="dc2e5-104">היכנס לניהול ההתקנים של Microsoft 365, ועבור אל **התקנים**של  >  **כל ההתקנים**.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="dc2e5-105">בחר את ההתקן שברצונך למחוק.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="dc2e5-106">בחר את סוג המחיקה המרוחקת שברצונך לבצע.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="dc2e5-107">הפרישה מוחקת רק מידע ארגוני, בעוד שמחיקות מלאות מחזירות את ההתקן להגדרות המפעל שלו.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="dc2e5-108">בחר **כן** כדי לאשר.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="dc2e5-109">עד לסיום המחיקה, מצב פעולת ההתקן מוצג כממתין לפרישה.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="dc2e5-110">לאחר השלמת הפעולה, לא תראה עוד את המכשיר הנייד ברשימת ההתקנים המנוהלים.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="dc2e5-111">**שים לב** אין אפשרות להסיר את נתוני החברה ממכשירים המצורפים לתכלת המודעה.</span><span class="sxs-lookup"><span data-stu-id="dc2e5-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="dc2e5-112">לקבלת פרטים מלאים על ההשפעה של פעולות הפרישה והמחיקה, כולל מה שנשמר ומה נמחק, ראה [הסרת התקנים באמצעות ניגוב, פרישה או ביטול הרישום של ההתקן באופן ידני](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="dc2e5-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="dc2e5-113">כדי למחוק את כל הנתונים מהתקן macOS, ראה [מחיקת כל הנתונים מהתקן macos](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="dc2e5-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>