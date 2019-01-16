---
title: פתרון בעיות עם רושם התקני Windows ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292694"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f4eb4-102">פתרון בעיות עם רושם התקני Windows ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f4eb4-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f4eb4-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="f4eb4-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f4eb4-104">כמה הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="f4eb4-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f4eb4-p101">**אין אפשרות להתקין את התוכנה, 0x80cf4017:** פג תוקפו של האישור לחשבון שלך. להוריד מחדש את חבילת התוכנה הלקוח מחשב אישי במסוף הניהול Intune. סקירת תיעוד זה לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="f4eb4-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="f4eb4-108">**קוד השגיאה 0x801c0003:** השגיאה עלולה להתרחש בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f4eb4-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="f4eb4-p102">למשתמש יש יותר התקנים שנרשמו ממגבלת המכשיר. סקירת מסמכים אלה כדי [להסיר התקן](https://docs.microsoft.com/en-us/intune/devices-wipe) או [לשנות את מגבלת התקן](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f4eb4-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="f4eb4-p103">"משתמשים עשויים להצטרף התקנים כדי AD תכלת הרקיע" מוגדרת ל- "none". להגדיר אותו לכל או בחר משתמשים. סקירת [תיעוד זה](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="f4eb4-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="f4eb4-p104">ההתקן כבר נרשם על-ידי משתמש אחר. אם זהו המקרה, הסר את ההתקן מהמסוף תכלת הרקיע Intune או unenroll את ההתקן באופן ידני לפני שתנסה שוב.</span><span class="sxs-lookup"><span data-stu-id="f4eb4-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="f4eb4-p105">ההתקן הוא 10 Windows Home. רק Pro 10 של Windows, חינוך ואת פריטי ה-Sku של הארגון יכולים להצטרף תכלת הרקיע Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f4eb4-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="f4eb4-118">משאבים נוספים כדי לסייע לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="f4eb4-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f4eb4-p106">להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות. סקירת [מסמך זה](https://docs.microsoft.com/en-us/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="f4eb4-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f4eb4-121">סקירת מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל: [מדריך פתרון בעיות](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ו- [doc ופתרון בעיות](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f4eb4-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="f4eb4-122">[למד כיצד לרשום התקני Windows Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f4eb4-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

