---
title: פתרון בעיות ברישום התקני אנדרואיד ב-Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759621"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d6a12-102">פתרון בעיות ברישום התקני אנדרואיד ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d6a12-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d6a12-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה שלך כעת.</span><span class="sxs-lookup"><span data-stu-id="d6a12-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d6a12-104">מספר שלבים נפוצים של בעיות ורזולוציות:</span><span class="sxs-lookup"><span data-stu-id="d6a12-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d6a12-105">**התקן לא שגיאה מוצפנת בפורטל החברה:** גירסאות חדשות יותר של Android, המתחילות במיוחד ב-v 7.0, דורשות קוד סיסמה של הפעלה כדי לוודא שההתקן שלך מוצפן במלואו.</span><span class="sxs-lookup"><span data-stu-id="d6a12-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d6a12-106">פתרונות נפוצים הם לאפשר לפין הפעלה או להצפין את ההתקן במלואו.</span><span class="sxs-lookup"><span data-stu-id="d6a12-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d6a12-107">עיין [במסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="d6a12-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d6a12-108">**התקנים אינם מצליחים לבצע צ'ק-אין בשירות Intune או להציג אותם כ"בלתי בריאים" במסוף מנהל Intune:** חלק סמסונג 4.4 ו-5.5 התקנים עשויים לא לבדוק את השירות.</span><span class="sxs-lookup"><span data-stu-id="d6a12-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d6a12-109">קיימים 3 פתרונות אפשריים לבעיה זו:</span><span class="sxs-lookup"><span data-stu-id="d6a12-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d6a12-110">פתח באופן ידני את יישום הפורטל של Intune Company, אשר תיזום באופן אוטומטי סינכרון התקן.</span><span class="sxs-lookup"><span data-stu-id="d6a12-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d6a12-111">עדכן את המכשיר אנדרואיד 6.0 או יותר.</span><span class="sxs-lookup"><span data-stu-id="d6a12-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d6a12-112">להשבית את סמסונג מנהל חכם מניהול פורטל החברה Intune.</span><span class="sxs-lookup"><span data-stu-id="d6a12-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d6a12-113">עיין [במסמך זה](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים אודות בעיות והחלטות אלה.</span><span class="sxs-lookup"><span data-stu-id="d6a12-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d6a12-114">**סוג רשיון משתמש לא חוקי** או **שם משתמש לא זוהה שגיאה:** יש להקצות למשתמש רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="d6a12-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d6a12-115">סקור מסמכים אלה כדי להקצות רשיון באמצעות: מרכז הניהול של Office או פורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="d6a12-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d6a12-116">משאבים נוספים שיסייעו בפתרון הבעיה:</span><span class="sxs-lookup"><span data-stu-id="d6a12-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d6a12-117">השתמש [בפורטל לפתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים נפוצים בהרשמה.</span><span class="sxs-lookup"><span data-stu-id="d6a12-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d6a12-118">לפרטים נוספים, עיין [במסמך זה](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="d6a12-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d6a12-119">סקור [מסמך זה](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות המונעות כל אחת מההרשמה והרזולוציות.</span><span class="sxs-lookup"><span data-stu-id="d6a12-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d6a12-120">[למד כיצד לרשום התקנים אנדרואיד ב-Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d6a12-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
