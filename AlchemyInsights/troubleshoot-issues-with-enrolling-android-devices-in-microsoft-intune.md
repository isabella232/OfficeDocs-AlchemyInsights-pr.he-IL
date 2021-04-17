---
title: פתרון בעיות ברישום מכשירי Android ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830943"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d0ddb-102">פתרון בעיות ברישום מכשירי Android ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d0ddb-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d0ddb-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d0ddb-104">כמה בעיות נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="d0ddb-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d0ddb-105">**שגיאת התקן לא מוצפנת בפורטל החברה:** גירסאות חדשות יותר של Android, במיוחד החל מ- v7.0, דורשות קוד סיסמה לאתחול כדי לוודא שהמכשיר שלך מוצפן באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d0ddb-106">פתרונות נפוצים הם לאפשר הצמדת אתחול או להצפין את המכשיר באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d0ddb-107">סקור [מסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d0ddb-108">ההתקנים לא מצליחים לבצע צ'ק-אין עם שירות Intune או להציג אותם **כ- "Unhealthy" במסוף הניהול של Intune:** ייתכן שמכשירים מסוימים של Samsung 4.4 ו- 5.5 לא יבדקו את השירות.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d0ddb-109">קיימים 3 פתרונות אפשריים לבעיה זו:</span><span class="sxs-lookup"><span data-stu-id="d0ddb-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d0ddb-110">פתח באופן ידני את האפליקציה Intune Company Portal, אשר תפעיל באופן אוטומטי סינכרון מכשיר.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d0ddb-111">עדכן את המכשיר ל- Android 6.0 ואילך.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d0ddb-112">הפוך את Samsung Smart Manager ללא זמין בניהול הפורטל של Intune Company.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d0ddb-113">סקור [מסמך זה](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים על בעיות ופתרונות אלה.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d0ddb-114">**סוג רשיון משתמש לא** חוקי או שגיאה בשם משתמש שאינו **מזוהה:** יש להקצות למשתמש רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d0ddb-115">סקור מסמכים אלה כדי להקצות רשיון באמצעות: מרכז הניהול של Office או פורטל Azure.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d0ddb-116">משאבים נוספים שיעזור לך לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="d0ddb-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d0ddb-117">השתמש [בפורטל פתרון הבעיות של Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלי הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d0ddb-118">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d0ddb-119">סקור [מסמך זה](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות שמונעות הרשמה ופתרונות לכל אחת מהשגיאות.</span><span class="sxs-lookup"><span data-stu-id="d0ddb-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d0ddb-120">[למד כיצד לרשום מכשירי Android ב- Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d0ddb-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
