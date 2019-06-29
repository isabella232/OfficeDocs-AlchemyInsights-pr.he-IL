---
title: פתרון בעיות עם רושם התקנים Android ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367290"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="e4cbc-102">פתרון בעיות עם רושם התקנים Android ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e4cbc-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="e4cbc-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e4cbc-104">מספר בעיות נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="e4cbc-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="e4cbc-105">**בהתקן אינם מוצפנים שגיאה בפורטל החברה:** גירסאות חדשות יותר של Android, v7.0, במיוחד החל לדרוש passcode האתחול כדי לוודא כי ההתקן שלך מוצפן באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="e4cbc-106">פתרונות נפוצים הם כדי להפוך pin האתחול או להצפין את ההתקן באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="e4cbc-107">סקירת [מסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="e4cbc-108">**התקנים להיכשל לבדוק באמצעות השירות Intune או להציג כ- "Unhealthy" במסוף הניהול Intune:** 4.4 Samsung מסוימים והתקני 5.5 ייתכן תסמן לתוך השירות.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="e4cbc-109">ישנם 3 פתרונות אפשריים לבעיה זו:</span><span class="sxs-lookup"><span data-stu-id="e4cbc-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="e4cbc-110">פתח app פורטל החברה Intune, אשר באופן אוטומטי יאתחל סינכרון ההתקן באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="e4cbc-111">עדכן את ההתקן כדי Android 6.0 ומעלה.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="e4cbc-112">ביטול מנהל חכם Samsung מניהול הפורטל החברה Intune.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="e4cbc-113">סקירת [מסמך זה](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים על בעיות ופתרונות אלה.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="e4cbc-114">**סוג חוקי של רשיון משתמש** או **משתמש שם לא מזוהה שגיאה:** שעל המשתמש שיש להקצות רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e4cbc-115">סקירת מסמכים אלה כדי להקצות רשיון דרך: פורטל מרכז הניהוליים של Office או תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="e4cbc-116">משאבים נוספים כדי לסייע לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="e4cbc-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e4cbc-117">להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e4cbc-118">סקירת [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="e4cbc-119">סקירת [מסמך זה](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל.</span><span class="sxs-lookup"><span data-stu-id="e4cbc-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="e4cbc-120">[למד כיצד לרשום התקנים Android ב- Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="e4cbc-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
