---
title: פתרון בעיות ברישום מכשירי Windows ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658879"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="c4089-102">פתרון בעיות ברישום מכשירי Windows ב-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="c4089-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="c4089-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="c4089-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c4089-104">מספר הודעות שגיאה נפוצות ושלבי פתרון:</span><span class="sxs-lookup"><span data-stu-id="c4089-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="c4089-105">**אין אפשרות להתקין את התוכנה, 0x80cf4017:** פג תוקפו של אישור החשבון שלך.</span><span class="sxs-lookup"><span data-stu-id="c4089-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="c4089-106">הורד מחדש את חבילת תוכנת לקוח של PC במסוף הניהול של המנגינה.</span><span class="sxs-lookup"><span data-stu-id="c4089-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="c4089-107">עיין בתיעוד זה לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="c4089-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="c4089-108">**קוד שגיאה 0x801c0003:** השגיאה עשויה להתרחש בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="c4089-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="c4089-109">המשתמש מכיל מכשירים נוספים שנרשמו ממגבלת ההתקן.</span><span class="sxs-lookup"><span data-stu-id="c4089-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c4089-110">סקור מסמכים אלה כדי [להסיר מכשיר](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c4089-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="c4089-111">"משתמשים עשויים להצטרף למכשירים לתכלת לספירה" מוגדר ל-"none".</span><span class="sxs-lookup"><span data-stu-id="c4089-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="c4089-112">הגדר הכל או בחר משתמשים.</span><span class="sxs-lookup"><span data-stu-id="c4089-112">Set it to all or select users.</span></span> <span data-ttu-id="c4089-113">עיין [בתיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="c4089-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="c4089-114">המכשיר כבר נרשם על-ידי משתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="c4089-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="c4089-115">אם זהו המצב, הסר את ההתקן מהמסוף של ' שינוי תכלת ' או בטל את הרישום של המכשיר באופן ידני לפני שתנסה שוב.</span><span class="sxs-lookup"><span data-stu-id="c4089-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="c4089-116">המכשיר הוא Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="c4089-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="c4089-117">רק מחשבי Sku של Windows 10 Pro, השכלה וארגונים יכולים להצטרף לתכלת Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c4089-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="c4089-118">משאבים נוספים שיעזרו לך לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="c4089-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="c4089-119">השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="c4089-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c4089-120">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="c4089-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="c4089-121">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ולפתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c4089-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="c4089-122">[למד כיצד לרשום מכשירי Windows ב-Microsoft intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="c4089-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
