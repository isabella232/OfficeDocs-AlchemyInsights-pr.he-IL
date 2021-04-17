---
title: פתרון בעיות ברישום מכשירי iOS ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823464"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="71b85-102">פתרון בעיות ברישום מכשירי iOS ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="71b85-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="71b85-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="71b85-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="71b85-104">כמה הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="71b85-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="71b85-105">**הגעת למכסה המכשיר** למשתמש יש יותר מכשירים שנרשמו ממגבלת המכשיר.</span><span class="sxs-lookup"><span data-stu-id="71b85-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="71b85-106">סקור מסמכים אלה כדי להסיר [מכשיר או לשנות](https://docs.microsoft.com/intune/devices-wipe) את [מגבלת המכשיר.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="71b85-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="71b85-107">**שירות זה אינו נתמך. אין צורך לקבוע את התצורה** או החידוש של שירות הודעות דחיפה (APNS) של Apple.</span><span class="sxs-lookup"><span data-stu-id="71b85-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="71b85-108">עיין [במסמך](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) זה לקבלת הוראות כיצד לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="71b85-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="71b85-109">**סוג רשיון משתמש לא חוקי או שם משתמש אינו מזוהה:** יש להקצות למשתמש רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="71b85-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="71b85-110">סקור מסמכים אלה כדי להקצות רשיון באמצעות: [מרכז הניהול של Office או](https://docs.microsoft.com/intune/licenses-assign) פורטל [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="71b85-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="71b85-111">משאבים נוספים שיעזור לך לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="71b85-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="71b85-112">השתמש [בפורטל פתרון הבעיות של Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלי הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="71b85-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="71b85-113">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="71b85-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="71b85-114">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות שמונעות הרשמה ופתרונות לכל אחד מהם: [מדריך פתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ומסמך לפתרון בעיות.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="71b85-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="71b85-115">[למד כיצד לרשום מכשירי iOS ב- Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="71b85-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

