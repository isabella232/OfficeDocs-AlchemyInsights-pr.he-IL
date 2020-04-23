---
title: פתרון בעיות ברישום התקני iOS ב-Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736159"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="3a0a6-102">פתרון בעיות ברישום התקני iOS ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3a0a6-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="3a0a6-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה שלך כעת.</span><span class="sxs-lookup"><span data-stu-id="3a0a6-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="3a0a6-104">מספר הודעות שגיאה נפוצות ושלבי פענוח:</span><span class="sxs-lookup"><span data-stu-id="3a0a6-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="3a0a6-105">**הגעת למכסה ההתקן** למשתמש יש התקנים נוספים שנרשמו ממגבלת ההתקן.</span><span class="sxs-lookup"><span data-stu-id="3a0a6-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3a0a6-106">סקור [מסמכים אלה כדי להסיר התקן](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="3a0a6-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="3a0a6-107">**שירות זה אינו נתמך. אין מדיניות הרשמה:** שירות הודעות לדחיפת Apple (APNS) צריך להיות מוגדר או מתחדש.</span><span class="sxs-lookup"><span data-stu-id="3a0a6-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="3a0a6-108">עיין [במסמך זה](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) לקבלת הוראות כיצד לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="3a0a6-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="3a0a6-109">**סוג רשיון משתמש לא חוקי או שם משתמש לא זוהה:** יש להקצות למשתמש רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="3a0a6-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3a0a6-110">סקור מסמכים אלה כדי להקצות רשיון באמצעות: [מרכז הניהול של Office](https://docs.microsoft.com/intune/licenses-assign) או [פורטל התכלת](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="3a0a6-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="3a0a6-111">משאבים נוספים שיסייעו בפתרון הבעיה:</span><span class="sxs-lookup"><span data-stu-id="3a0a6-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3a0a6-112">השתמש [בפורטל לפתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים נפוצים בהרשמה.</span><span class="sxs-lookup"><span data-stu-id="3a0a6-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3a0a6-113">לפרטים נוספים, עיין [במסמך זה](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="3a0a6-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="3a0a6-114">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה והחלטות לכל: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ולפתרון בעיות doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="3a0a6-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="3a0a6-115">[למד כיצד לרשום התקני iOS ב-Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="3a0a6-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

