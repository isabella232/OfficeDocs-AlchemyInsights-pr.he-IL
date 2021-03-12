---
title: פתרון בעיות ברישום מכשירי iOS ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708963"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="ad263-102">פתרון בעיות ברישום מכשירי iOS ב-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="ad263-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="ad263-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="ad263-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ad263-104">מספר הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="ad263-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="ad263-105">**הגעת לאות המכשירים** המשתמש מכיל מכשירים נוספים שנרשמו ממגבלת ההתקן.</span><span class="sxs-lookup"><span data-stu-id="ad263-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ad263-106">סקור מסמכים אלה כדי [להסיר מכשיר](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ad263-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="ad263-107">**שירות זה אינו נתמך. ללא מדיניות הרשמה:** שירות ההודעות של Apple פוש (APNS) צריך להיות מוגדר או מתחדש.</span><span class="sxs-lookup"><span data-stu-id="ad263-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="ad263-108">סקור [מסמך זה](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) לקבלת הוראות לביצוע פעולה זו.</span><span class="sxs-lookup"><span data-stu-id="ad263-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="ad263-109">**סוג רשיון משתמש לא חוקי או שם משתמש אינו מזוהה:** יש להקצות למשתמש רשיון כוונון או EMS.</span><span class="sxs-lookup"><span data-stu-id="ad263-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ad263-110">סקור מסמכים אלה כדי להקצות רשיון דרך: [מרכז הניהול של Office](https://docs.microsoft.com/intune/licenses-assign) או [פורטל התכלת](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="ad263-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="ad263-111">משאבים נוספים שיעזרו לך לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="ad263-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ad263-112">השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="ad263-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ad263-113">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="ad263-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ad263-114">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ולפתרון בעיות](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ad263-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="ad263-115">[למד כיצד לרשום מכשירי iOS ב-Microsoft intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="ad263-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

