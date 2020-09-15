---
title: פתרון בעיות ברישום מכשירי Android ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689955"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="2bec6-102">פתרון בעיות ברישום מכשירי Android ב-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="2bec6-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="2bec6-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="2bec6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="2bec6-104">כמה בעיות נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="2bec6-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="2bec6-105">**שגיאה לא מוצפנת של התקן בפורטל החברה:** גירסאות חדשות יותר של Android, במיוחד החל מ-v 7.0, דורשות סיסמה של הפעלה כדי לוודא שההתקן שלך מוצפן במלואו.</span><span class="sxs-lookup"><span data-stu-id="2bec6-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="2bec6-106">פתרונות נפוצים משמשים להפיכת מספר זיהוי אישי של הפעלה לזמין או להצפנה מלאה של המכשיר.</span><span class="sxs-lookup"><span data-stu-id="2bec6-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="2bec6-107">סקור [מסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="2bec6-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="2bec6-108">**המכשירים אינם מצליחים להיכנס באמצעות שירות ה-intune או הצג כ-"לא בריא" במסוף הניהול של intune:** ייתכן שמכשירים מסוימים של Samsung 4.4 ו-5.5 לא ייכנסו לשירות.</span><span class="sxs-lookup"><span data-stu-id="2bec6-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="2bec6-109">קיימים 3 פתרונות אפשריים לבעיה זו:</span><span class="sxs-lookup"><span data-stu-id="2bec6-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="2bec6-110">פתח באופן ידני את יישום הפורטל של כוונון החברה, שייזום באופן אוטומטי סינכרון מכשיר.</span><span class="sxs-lookup"><span data-stu-id="2bec6-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="2bec6-111">עדכן את המכשיר ל-Android 6.0 ואילך.</span><span class="sxs-lookup"><span data-stu-id="2bec6-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="2bec6-112">הפוך את סמסונג Smart Manager ללא זמין מניהול הפורטל של החברה.</span><span class="sxs-lookup"><span data-stu-id="2bec6-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="2bec6-113">סקור [מסמך זה](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים על בעיות ופתרונות אלה.</span><span class="sxs-lookup"><span data-stu-id="2bec6-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="2bec6-114">**סוג רשיון של משתמש לא חוקי** או **שם משתמש לא זוהה שגיאה:** המשתמש צריך להקצות לו רשיון של כוונון או EMS.</span><span class="sxs-lookup"><span data-stu-id="2bec6-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2bec6-115">סקור מסמכים אלה כדי להקצות רשיון דרך: מרכז הניהול של Office או פורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="2bec6-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="2bec6-116">משאבים נוספים שיעזרו לך לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="2bec6-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2bec6-117">השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="2bec6-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2bec6-118">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="2bec6-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="2bec6-119">סקור [מסמך זה](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן.</span><span class="sxs-lookup"><span data-stu-id="2bec6-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="2bec6-120">[למד כיצד לרשום מכשירים של Android ב-Microsoft intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="2bec6-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
