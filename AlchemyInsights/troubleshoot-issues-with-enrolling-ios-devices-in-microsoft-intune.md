---
title: פתרון בעיות עם רושם iOS התקנים ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391008"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="05c61-102">פתרון בעיות עם רושם iOS התקנים ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="05c61-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="05c61-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="05c61-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="05c61-104">כמה הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="05c61-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="05c61-105">**כיפה ההתקן הגיע** למשתמש יש יותר התקנים שנרשמו ממגבלת המכשיר.</span><span class="sxs-lookup"><span data-stu-id="05c61-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="05c61-106">סקירת מסמכים אלה כדי [להסיר התקן](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת התקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="05c61-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="05c61-107">**שירות זה אינו נתמך. אין מדיניות הרשמה:** תפוח לדחוף דיווח שירות (ולמפעיל) צריך להיות מוגדר או לחדש.</span><span class="sxs-lookup"><span data-stu-id="05c61-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="05c61-108">סקירת [מסמך זה](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) לקבלת הוראות אודות אופן ביצוע פעולה זו.</span><span class="sxs-lookup"><span data-stu-id="05c61-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="05c61-109">**סוג רשיון משתמש לא חוקי או לא מזוהה שם משתמש:** המשתמש צריך להקצות רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="05c61-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="05c61-110">סקירת מסמכים אלה כדי להקצות רשיון דרך: [מרכז הניהוליים של Office](https://docs.microsoft.com/intune/licenses-assign) או [פורטל תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="05c61-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="05c61-111">משאבים נוספים כדי לסייע לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="05c61-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="05c61-112">להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות.</span><span class="sxs-lookup"><span data-stu-id="05c61-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="05c61-113">סקירת [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="05c61-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="05c61-114">סקירת מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל: [מדריך פתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ו- [doc ופתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="05c61-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="05c61-115">[למד כיצד לרשום iOS התקנים ב- Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="05c61-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

