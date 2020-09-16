---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731240"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="900a3-102">הפעלת הצפנת Bitlocker באמצעות ' כוונון '</span><span class="sxs-lookup"><span data-stu-id="900a3-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="900a3-103">ניתן להשתמש במדיניות הגנה מפני נקודות קצה כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור מכשירי Windows.</span><span class="sxs-lookup"><span data-stu-id="900a3-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="900a3-104">לקבלת מידע נוסף, ראה [הגדרות Windows 10 (ואילך) כדי להגן על מכשירים באמצעות ' כוונון](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)'.</span><span class="sxs-lookup"><span data-stu-id="900a3-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="900a3-105">עליך להיות מודע לכך שמכשירים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, שמופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="900a3-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="900a3-106">פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן ברירות מחדל נקבעו.</span><span class="sxs-lookup"><span data-stu-id="900a3-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="900a3-107">עיין בשאלות הנפוצות הבאות לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="900a3-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="900a3-108">לקבלת מידע אודות פתרון בעיות ב-bitlocker, ראה [פתרון בעיות במדיניות bitlocker ב-Microsoft intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="900a3-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="900a3-109">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="900a3-109">**FAQ**</span></span>

 <span data-ttu-id="900a3-110">ש: אילו מהדורות של הצפנת מכשירים של Windows תומכת באמצעות מדיניות הגנה על נקודות קצה?</span><span class="sxs-lookup"><span data-stu-id="900a3-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="900a3-111">ת: ההגדרות במדיניות הגנה על נקודות הקצה מתבצעות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="900a3-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="900a3-112">לא כל המהדורות או גירסאות build של Windows תומכות ב-CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="900a3-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="900a3-113">בשלב זה, המהדורות הבאות של Windows נתמכות: Enterprise, השכלה, Mobile, Mobile Enterprise ו-Professional (גירסת build מס ' 1809 ואילך).</span><span class="sxs-lookup"><span data-stu-id="900a3-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="900a3-114">ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה ועוצמת הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="900a3-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="900a3-115">תשובה: לא.</span><span class="sxs-lookup"><span data-stu-id="900a3-115">A: No.</span></span> <span data-ttu-id="900a3-116">כדי להחיל את הגדרות הצופן החדשות, תחילה יש לפענח את הכונן.</span><span class="sxs-lookup"><span data-stu-id="900a3-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="900a3-117">**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכת מדיניות ההגדרה, המאפשרת שימוש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="900a3-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="900a3-118">ש: אם התקן מוצפן כתוצאה מתוך היישום של מדיניות ה-intune, האם היא תפענח כאשר מדיניות זו תוסר?</span><span class="sxs-lookup"><span data-stu-id="900a3-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="900a3-119">ת: הסרת מדיניות הקשורה להצפנה אינה מביאה לפענוח של הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="900a3-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="900a3-120">ש: מדוע מדיניות התאימות מציגה כי המכשיר שלי אינו מופעל על-ידי Bitlocker, למרות שהוא מופעל?</span><span class="sxs-lookup"><span data-stu-id="900a3-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="900a3-121">ת: ההגדרה "Bitlocker enabled" במדיניות התאימות של ' שימוש בעידון ' משתמשת בלקוח תקינות התקן של Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="900a3-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="900a3-122">לקוח זה מודד רק את מצב ההתקן בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="900a3-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="900a3-123">אז אם התקן לא אותחל מחדש מאז השלמת הצפנת Bitlocker, שירות הלקוח של DHA לא ידווח על Bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="900a3-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 