---
title: פתרון בעיות ברישום מכשירי Windows ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808972"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="1630b-102">פתרון בעיות ברישום מכשירי Windows ב- Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1630b-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="1630b-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="1630b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="1630b-104">כמה הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="1630b-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="1630b-105">**לא ניתן להתקין את התוכנה, 0x80cf4017:** פג תוקפו של אישור החשבון שלך.</span><span class="sxs-lookup"><span data-stu-id="1630b-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="1630b-106">הורד מחדש את חבילת התוכנה של לקוח PC במסוף הניהול של Intune.</span><span class="sxs-lookup"><span data-stu-id="1630b-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="1630b-107">עיין בתיעוד זה לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="1630b-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="1630b-108">**קוד שגיאה 0x801c0003:** השגיאה עשויה להתרחש בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1630b-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="1630b-109">למשתמש יש יותר מכשירים שנרשמו ממגבלת המכשיר.</span><span class="sxs-lookup"><span data-stu-id="1630b-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1630b-110">סקור מסמכים אלה כדי להסיר [מכשיר או לשנות](https://docs.microsoft.com/intune/devices-wipe) את [מגבלת המכשיר.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="1630b-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="1630b-111">"משתמשים עשויים להצטרף למכשירים ל- Azure AD" מוגדר ל- "none".</span><span class="sxs-lookup"><span data-stu-id="1630b-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="1630b-112">הגדר אותו לכל המשתמשים או בחר אותם.</span><span class="sxs-lookup"><span data-stu-id="1630b-112">Set it to all or select users.</span></span> <span data-ttu-id="1630b-113">עיין [בתיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="1630b-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="1630b-114">המכשיר כבר רשום על-ידי משתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="1630b-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="1630b-115">במקרה זה, הסר את המכשיר ממסוף Azure Intune או בטל את ההסתה של המכשיר באופן ידני לפני ניסיון שוב.</span><span class="sxs-lookup"><span data-stu-id="1630b-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="1630b-116">המכשיר הוא Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="1630b-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="1630b-117">רק Windows 10 Pro, Education ו- Enterprise SKUs יכולים להצטרף ל- Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1630b-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="1630b-118">משאבים נוספים שיעזור לך לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="1630b-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="1630b-119">השתמש [בפורטל פתרון הבעיות של Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלי הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="1630b-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1630b-120">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="1630b-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="1630b-121">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות שמונעות הרשמה ופתרונות לכל אחד מהם: [מדריך פתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ומסמך לפתרון בעיות.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="1630b-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="1630b-122">[למד כיצד לרשום מכשירי Windows ב- Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="1630b-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
