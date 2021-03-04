---
title: הסרת נתונים ומחיקת מכשירים מ- Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416314"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="f4694-102">הסרת נתונים ומחיקת מכשירים מ- Intune</span><span class="sxs-lookup"><span data-stu-id="f4694-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="f4694-103">ניתן להשתמש בפעולות מרוחקות של 'הוצאת מכשיר משימוש' ו'מחיקת מכשיר' כדי להסיר נתוני חברה שמונעלים על-ידי Intune או כדי לבצע איפוס יצרן ולהחזיר את המכשיר להגדרות ברירת המחדל שלו.</span><span class="sxs-lookup"><span data-stu-id="f4694-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="f4694-104">היכנס לניהול המכשירים של Microsoft 365 ועבור אל **מכשירים** > **כל המכשירים**.</span><span class="sxs-lookup"><span data-stu-id="f4694-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="f4694-105">בחר את ההתקן שברצונך למחוק.</span><span class="sxs-lookup"><span data-stu-id="f4694-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="f4694-106">בחר את הסוג של המחיקה מרחוק שברצונך לבצע.</span><span class="sxs-lookup"><span data-stu-id="f4694-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="f4694-107">הפעולה 'הוצא משימוש' מוחקת מידע ארגוני בלבד, בשעה שמחיקה מלאה משחזרת את המכשיר להגדרות היצרן שלו.</span><span class="sxs-lookup"><span data-stu-id="f4694-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="f4694-108">בחר **כן** כדי לאשר.</span><span class="sxs-lookup"><span data-stu-id="f4694-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="f4694-109">עד לסיום המחיקה, מצב הפעולה של המכשיר יופיע ג *הוצאה משימוש ממתינה*.</span><span class="sxs-lookup"><span data-stu-id="f4694-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="f4694-110">לאחר השלמת הפעולה, לא תראה עוד את המכשיר הנייד ברשימת המכשירים המנוהלים.</span><span class="sxs-lookup"><span data-stu-id="f4694-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="f4694-111">לא ניתן להסיר נתוני חברה ממכשירים שהצטרפו ל- Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4694-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="f4694-112">לקבלת פרטים מלאים של השפעת פעולות 'הוצאה משימוש' ו'מחיקה', כולל מה נשמר ומה נמחק, ראה את המסמכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f4694-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="f4694-113">[הסרת מכשירים על-ידי מחיקה, הוצאה משימוש או ביטול רישום של המכשיר](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="f4694-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="f4694-114">כיצד למחוק נתונים ארגוניים בלבד מאפליקציות המנוהלות על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="f4694-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="f4694-115">[מחיקת כל הנתונים ממכשיר macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="f4694-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>