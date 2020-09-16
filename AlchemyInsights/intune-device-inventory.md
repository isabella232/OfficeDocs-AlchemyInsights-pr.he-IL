---
title: כוונון מלאי מכשיר
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667879"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="0828d-102">כוונון מלאי מכשיר</span><span class="sxs-lookup"><span data-stu-id="0828d-102">Intune Device Inventory</span></span>

<span data-ttu-id="0828d-103">להב המכשירים מספק את התובנה של מנהל המערכת במכשירים מתחת לניהול באמצעות המנגינה על בסיס כל מכשיר.</span><span class="sxs-lookup"><span data-stu-id="0828d-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="0828d-104">המידע המוצג כולל: חומרה, יישומים מאותרים, מצב תאימות התקן ומצב תצורת התקן.</span><span class="sxs-lookup"><span data-stu-id="0828d-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="0828d-105">נתוני מלאי עבור חומרה ויישומים שאותרו נאספים במחזור של שבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="0828d-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="0828d-106">היישומים ורכיבי החומרה הספציפיים שדווחו משתנים בהתאם למערכת ההפעלה של ההתקן ולשאלה אם ההתקן נמצא בבעלות אישית או חברה.</span><span class="sxs-lookup"><span data-stu-id="0828d-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="0828d-107">לקבלת מידע נוסף, ראה [הצגת פרטי התקן בתוך המנגינה](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="0828d-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="0828d-108">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="0828d-108">**FAQ**</span></span>

<span data-ttu-id="0828d-109">ש: איני מקבל רשימת מלאי מלאה של יישומים הקיימים במכשירי Windows שנרשמים כשהם מוצגים.</span><span class="sxs-lookup"><span data-stu-id="0828d-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="0828d-110">למה לא?</span><span class="sxs-lookup"><span data-stu-id="0828d-110">Why not?</span></span>

<span data-ttu-id="0828d-111">ת: בשלב זה, רק יישומים מודרניים מפורטים עבור מחשבי Windows 10 המזוהים כמכשירים של החברה.</span><span class="sxs-lookup"><span data-stu-id="0828d-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="0828d-112">המנגינה אינה אוספת מידע אודות יישומי Win32 המותקנים במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="0828d-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="0828d-113">ש: מדוע מספרי טלפון אינם נאספים מכל המכשירים?</span><span class="sxs-lookup"><span data-stu-id="0828d-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="0828d-114">א: טלפונים שסווגו כמכשירים של החברה בתוך ' שילוב ' אינם מזוהים עם מספר הטלפון המלא שלהם כאשר, לדוגמה, אתה מפעיל דוח מלאי מכשיר נייד.</span><span class="sxs-lookup"><span data-stu-id="0828d-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="0828d-115">מספרי טלפון של ' הבא ' שלך מצוידים תמיד במסיכה חלקית באמצעות כוכביות (\* \* \* \*) ומציגות רק את ארבע הספרות האחרונות.</span><span class="sxs-lookup"><span data-stu-id="0828d-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>