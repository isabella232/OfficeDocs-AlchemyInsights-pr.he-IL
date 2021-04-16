---
title: שכפול הרשומה של המכשיר בפורטל
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814517"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="51788-102">שכפול הרשומה של המכשיר בפורטל</span><span class="sxs-lookup"><span data-stu-id="51788-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="51788-103">ייתכן שתראה 2 רשומות עבור מכשיר בפורטל אם המכשיר לא מדווח כראוי על מצב הניהול המשותף לאתר מנהל התצורה.</span><span class="sxs-lookup"><span data-stu-id="51788-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="51788-104">כדי לבדוק את מצב הניהול המשותף של המכשיר, סקור את העמודה **'מנוהל במשותף'** עבור המכשיר במסוף מנהל התצורה.</span><span class="sxs-lookup"><span data-stu-id="51788-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="51788-105">אם העמודה אינה גלויה, תוכל להוסיף אותה על-ידי לחיצה באמצעות לחצן העכבר הימני על כל אחת מכותרות העמודות ובחירתה מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="51788-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="51788-106">הערך 'מנוהל במשותף' חייב להיות **'כן'**.</span><span class="sxs-lookup"><span data-stu-id="51788-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="51788-107">אם הערך הוא **'לא'**, פתח את יישומון הלקוח של מנהל התצורה במכשיר הלקוח ובדוק את המאפיין **'ניהול משותף'** בכרטיסיה כללי.</span><span class="sxs-lookup"><span data-stu-id="51788-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="51788-108">אם הערך הוא **'זמין'**, משמעות הדבר היא בעיות בתקשורת לקוח עם נקודת הניהול.</span><span class="sxs-lookup"><span data-stu-id="51788-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="51788-109">עיין ב **CcmMessaging.log** במכשיר כדי לחקור בעיות קישוריות פוטנציאליות.</span><span class="sxs-lookup"><span data-stu-id="51788-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="51788-110">אם הערך הוא **'לא זמין'** והמכשיר רשום באמצעות Intune, ודא שהמכשיר קיבל מדיניות ניהול משותף על-ידי סקירת **CoManagementHandler.log** במכשיר.</span><span class="sxs-lookup"><span data-stu-id="51788-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
