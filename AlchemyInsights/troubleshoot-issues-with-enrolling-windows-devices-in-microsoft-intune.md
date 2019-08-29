---
title: פתרון בעיות ברישום התקני Windows ב-Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665833"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="a9e00-102">פתרון בעיות ברישום התקני Windows ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a9e00-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="a9e00-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה שלך כעת.</span><span class="sxs-lookup"><span data-stu-id="a9e00-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a9e00-104">מספר הודעות שגיאה נפוצות ושלבי פענוח:</span><span class="sxs-lookup"><span data-stu-id="a9e00-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="a9e00-105">**לא ניתן להתקין את התוכנה, 0x80cf4017:** פג תוקפו של אישור החשבון שלך.</span><span class="sxs-lookup"><span data-stu-id="a9e00-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="a9e00-106">הורד מחדש את חבילת התוכנות PC Client במסוף Intune Admin.</span><span class="sxs-lookup"><span data-stu-id="a9e00-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="a9e00-107">עיין בתיעוד זה לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="a9e00-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="a9e00-108">**קוד שגיאה 0x801c0003:** השגיאה יכולה להופיע בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="a9e00-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="a9e00-109">למשתמש יש התקנים נוספים שנרשמו ממגבלת ההתקן.</span><span class="sxs-lookup"><span data-stu-id="a9e00-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a9e00-110">סקור מסמכים אלה [](https://docs.microsoft.com/intune/devices-wipe) כדי להסיר התקן או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a9e00-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="a9e00-111">"משתמשים יכולים לצרף התקנים לתכלת AD" מוגדר "none".</span><span class="sxs-lookup"><span data-stu-id="a9e00-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="a9e00-112">הגדר אותה לכל או בחר משתמשים.</span><span class="sxs-lookup"><span data-stu-id="a9e00-112">Set it to all or select users.</span></span> <span data-ttu-id="a9e00-113">עיין [בתיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="a9e00-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="a9e00-114">ההתקן כבר נרשם על-ידי משתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="a9e00-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="a9e00-115">אם זה המקרה, להסיר את המכשיר מהמסוף Intune תכלת או לבטל ידנית את הרישום של המכשיר לפני שתנסה שוב.</span><span class="sxs-lookup"><span data-stu-id="a9e00-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="a9e00-116">ההתקן הוא Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="a9e00-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="a9e00-117">רק Windows 10 Pro, השכלה וארגון SKUs יכול להצטרף כחול Active ספריה.</span><span class="sxs-lookup"><span data-stu-id="a9e00-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="a9e00-118">משאבים נוספים שיסייעו בפתרון הבעיה:</span><span class="sxs-lookup"><span data-stu-id="a9e00-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="a9e00-119">השתמש [בפורטל לפתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים נפוצים בהרשמה.</span><span class="sxs-lookup"><span data-stu-id="a9e00-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a9e00-120">לפרטים נוספים, עיין [במסמך זה](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="a9e00-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="a9e00-121">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה והחלטות לכל: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ולפתרון בעיות [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a9e00-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="a9e00-122">[למד כיצד לרשום התקני Windows ב-Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="a9e00-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
