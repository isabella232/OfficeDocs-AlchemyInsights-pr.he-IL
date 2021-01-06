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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768818"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="66637-102">הפעלת הצפנת Bitlocker באמצעות ' כוונון '</span><span class="sxs-lookup"><span data-stu-id="66637-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="66637-103">ניתן להשתמש במדיניות הגנה מפני נקודות קצה כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור מכשירי Windows.</span><span class="sxs-lookup"><span data-stu-id="66637-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="66637-104">לקבלת מידע נוסף, ראה [הגדרות Windows 10 (ואילך) כדי להגן על מכשירים באמצעות ' כוונון](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)'.</span><span class="sxs-lookup"><span data-stu-id="66637-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="66637-105">עליך להיות מודע לכך שמכשירים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, שמופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="66637-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="66637-106">פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן ברירות מחדל נקבעו.</span><span class="sxs-lookup"><span data-stu-id="66637-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="66637-107">עיין בשאלות הנפוצות הבאות לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="66637-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="66637-108">לקבלת מידע אודות פתרון בעיות ב-bitlocker, ראה [פתרון בעיות במדיניות bitlocker ב-Microsoft intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="66637-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="66637-109">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="66637-109">**FAQ**</span></span>

<span data-ttu-id="66637-110">ש: אילו מהדורות של הצפנת מכשירים של Windows תומכת באמצעות מדיניות הגנה על נקודות קצה?</span><span class="sxs-lookup"><span data-stu-id="66637-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="66637-111">ת: ההגדרות במדיניות הגנה על נקודות הקצה מתבצעות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="66637-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="66637-112">לא כל המהדורות או גירסאות build של Windows תומכות ב-CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="66637-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="66637-113">ש: כיצד ניתן להפוך את Bitlocker לזמין במכשירים מבלי לדרוש אינטראקציה של משתמשי קצה?</span><span class="sxs-lookup"><span data-stu-id="66637-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="66637-114">ת: כל עוד הדרישות הנדרשות מראש מתקיימות, ניתן להפוך את Bitlocker "למצב הצפנה שקט" באמצעות המנגינה.</span><span class="sxs-lookup"><span data-stu-id="66637-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="66637-115">עיין בפרטים של דרישות ההתקן והגדרות מדיניות לדוגמה כדי לאפשר הצפנה שקטה במסמך הבא: [הפיכת הצפנת Bitlocker לזמינה בצורה שקטה](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="66637-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="66637-116">ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה ועוצמת הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="66637-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="66637-117">תשובה: לא.</span><span class="sxs-lookup"><span data-stu-id="66637-117">A: No.</span></span> <span data-ttu-id="66637-118">כדי להחיל את הגדרות הצופן החדשות, תחילה יש לפענח את הכונן.</span><span class="sxs-lookup"><span data-stu-id="66637-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="66637-119">**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכת מדיניות ההגדרה, המאפשרת שימוש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="66637-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="66637-120">ש: אם התקן מוצפן כתוצאה מתוך היישום של מדיניות ה-intune, האם היא תפענח כאשר מדיניות זו תוסר?</span><span class="sxs-lookup"><span data-stu-id="66637-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="66637-121">ת: הסרת מדיניות הקשורה להצפנה אינה מביאה לפענוח של הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="66637-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="66637-122">ש: מדוע מדיניות התאימות מציגה כי המכשיר שלי אינו מופעל על-ידי Bitlocker, למרות שהוא מופעל?</span><span class="sxs-lookup"><span data-stu-id="66637-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="66637-123">ת: ההגדרה "Bitlocker enabled" במדיניות התאימות של ' שימוש בעידון ' משתמשת בלקוח תקינות התקן של Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="66637-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="66637-124">לקוח זה מודד רק את מצב ההתקן בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="66637-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="66637-125">אז אם התקן לא אותחל מחדש מאז השלמת הצפנת Bitlocker, שירות הלקוח של DHA לא ידווח על Bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="66637-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 