---
title: מלאי מכשירים Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439654"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="a0fb9-102">מלאי מכשירים Intune</span><span class="sxs-lookup"><span data-stu-id="a0fb9-102">Intune Device Inventory</span></span>

<span data-ttu-id="a0fb9-103">הלהב Devices מספק את התובנה של מנהל מערכת בהתקנים תחת ניהול ב-Intune על בסיס כל התקן.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="a0fb9-104">המידע המוצג כולל: חומרה, יישומים שהתגלו, מצב תאימות התקנים ומצב תצורת התקן.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="a0fb9-105">נתוני מלאי עבור חומרה ויישומים שהתגלו נאספים במחזור של שבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="a0fb9-106">היישומים והרכיבים הספציפיים של החומרה שדווחו שונים בהתאם למערכת ההפעלה של ההתקן ולשאלה אם ההתקן הוא אישי או בבעלות חברה.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="a0fb9-107">לקבלת מידע נוסף, ראה [ראה פרטי התקן ב-Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="a0fb9-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="a0fb9-108">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="a0fb9-108">**FAQ**</span></span>

<span data-ttu-id="a0fb9-109">ש: אני לא מקבל רשימת מלאי מלאה של יישומים הנמצאים בIntune התקנים של Windows שנרשמו.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="a0fb9-110">למה לא?</span><span class="sxs-lookup"><span data-stu-id="a0fb9-110">Why not?</span></span>

<span data-ttu-id="a0fb9-111">ת: בשלב זה, רק אפליקציות מודרניות מפורטות עבור Windows 10 PCs המזוהים כהתקנים ארגוניים.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="a0fb9-112">Intune אינו אוסף מידע אודות יישומי Win32 המותקנים במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="a0fb9-113">ש: מדוע לא נאספים מספרי טלפון מכל המכשירים?</span><span class="sxs-lookup"><span data-stu-id="a0fb9-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="a0fb9-114">ת: טלפונים המסווגים כהתקנים ארגוניים ב-Intune אינם מזוהים עם מספר הטלפון המלא שלהם כאשר, לדוגמה, אתה מפעיל דוח מלאי של התקן נייד.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="a0fb9-115">מספרי טלפון בהתקן הבא-לך-התקן מוסתרים תמיד באופן חלקי עם כוכביות (\* \* \* \*) ומציגות רק את ארבע הספרות האחרונות.</span><span class="sxs-lookup"><span data-stu-id="a0fb9-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>