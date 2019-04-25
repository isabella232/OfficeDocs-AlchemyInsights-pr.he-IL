---
title: פתרון בעיות עם רושם התקני Windows ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390644"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="daa3b-102">פתרון בעיות עם רושם התקני Windows ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="daa3b-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="daa3b-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="daa3b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="daa3b-104">כמה הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="daa3b-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="daa3b-105">**אין אפשרות להתקין את התוכנה, 0x80cf4017:** פג תוקפו של האישור לחשבון שלך.</span><span class="sxs-lookup"><span data-stu-id="daa3b-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="daa3b-106">להוריד מחדש את חבילת התוכנה הלקוח מחשב אישי במסוף הניהול Intune.</span><span class="sxs-lookup"><span data-stu-id="daa3b-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="daa3b-107">סקירת תיעוד זה לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="daa3b-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="daa3b-108">**קוד השגיאה 0x801c0003:** השגיאה עלולה להתרחש בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="daa3b-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="daa3b-109">למשתמש יש יותר התקנים שנרשמו ממגבלת המכשיר.</span><span class="sxs-lookup"><span data-stu-id="daa3b-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="daa3b-110">סקירת מסמכים אלה כדי [להסיר התקן](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת התקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="daa3b-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="daa3b-111">"משתמשים עשויים להצטרף התקנים כדי AD תכלת הרקיע" מוגדרת ל- "none".</span><span class="sxs-lookup"><span data-stu-id="daa3b-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="daa3b-112">להגדיר אותו לכל או בחר משתמשים.</span><span class="sxs-lookup"><span data-stu-id="daa3b-112">Set it to all or select users.</span></span> <span data-ttu-id="daa3b-113">סקירת [תיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="daa3b-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="daa3b-114">ההתקן כבר נרשם על-ידי משתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="daa3b-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="daa3b-115">אם זהו המקרה, הסר את ההתקן מהמסוף תכלת הרקיע Intune או unenroll את ההתקן באופן ידני לפני שתנסה שוב.</span><span class="sxs-lookup"><span data-stu-id="daa3b-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="daa3b-116">ההתקן הוא 10 Windows Home.</span><span class="sxs-lookup"><span data-stu-id="daa3b-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="daa3b-117">רק Pro 10 של Windows, חינוך ואת פריטי ה-Sku של הארגון יכולים להצטרף תכלת הרקיע Active Directory.</span><span class="sxs-lookup"><span data-stu-id="daa3b-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="daa3b-118">משאבים נוספים כדי לסייע לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="daa3b-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="daa3b-119">להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות.</span><span class="sxs-lookup"><span data-stu-id="daa3b-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="daa3b-120">סקירת [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="daa3b-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="daa3b-121">סקירת מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל: [מדריך פתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ו- [doc ופתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="daa3b-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="daa3b-122">[למד כיצד לרשום התקני Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="daa3b-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

