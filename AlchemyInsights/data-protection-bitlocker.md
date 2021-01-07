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
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778194"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="01878-102">הפעלת הצפנת Bitlocker באמצעות ' כוונון '</span><span class="sxs-lookup"><span data-stu-id="01878-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="01878-103">ניתן להשתמש במדיניות הגנה מפני נקודות קצה כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור מכשירי Windows.</span><span class="sxs-lookup"><span data-stu-id="01878-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="01878-104">לקבלת מידע נוסף, ראה [הגדרות Windows 10 (ואילך) כדי להגן על מכשירים באמצעות ' כוונון](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)'.</span><span class="sxs-lookup"><span data-stu-id="01878-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="01878-105">בנוסף למדיניות הגנה על נקודות קצה, יש גם דוח הצפנה המספק תצוגה מפורטת יותר של מצב ההצפנה עבור המכשירים.</span><span class="sxs-lookup"><span data-stu-id="01878-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="01878-106">ניתן לגשת לדוח זה מתוך פורטל הזיכרון תחת **מכשירים > צג** ולאחר מכן, תחת **קביעת תצורה** , בחר [דוח הצפנה](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span><span class="sxs-lookup"><span data-stu-id="01878-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="01878-107">אם אתה מגלה ש-Bitlocker אינו זמין כצפוי או שהפרופיל המשמש להפיכת Bitlocker לזמין נמצא במצב שגיאה, עיין בדוח ההצפנה כדי להבין טוב יותר את הסיבה לכך שההתנהגות מתרחשת.</span><span class="sxs-lookup"><span data-stu-id="01878-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="01878-108">לקבלת פרטים אודות אופן הפענוח של הדוח, כולל ערכי מצב ההצפנה השונים, ראה [פיקוח על הצפנת מכשירים באמצעות ' כוונון](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)'.</span><span class="sxs-lookup"><span data-stu-id="01878-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="01878-109">עליך להיות מודע לכך שמכשירים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, שמופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="01878-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="01878-110">פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן ברירות מחדל נקבעו.</span><span class="sxs-lookup"><span data-stu-id="01878-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="01878-111">עיין בשאלות הנפוצות הבאות לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="01878-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="01878-112">לקבלת מידע אודות פתרון בעיות ב-bitlocker, ראה [פתרון בעיות במדיניות bitlocker ב-Microsoft intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="01878-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="01878-113">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="01878-113">**FAQ**</span></span>

<span data-ttu-id="01878-114">ש: אילו מהדורות של הצפנת מכשירים של Windows תומכת באמצעות מדיניות הגנה על נקודות קצה?</span><span class="sxs-lookup"><span data-stu-id="01878-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="01878-115">ת: ההגדרות במדיניות הגנה על נקודות הקצה מתבצעות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="01878-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="01878-116">לא כל המהדורות או גירסאות build של Windows תומכות ב-CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="01878-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="01878-117">ש: כיצד ניתן להפוך את Bitlocker לזמין במכשירים מבלי לדרוש אינטראקציה של משתמשי קצה?</span><span class="sxs-lookup"><span data-stu-id="01878-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="01878-118">ת: כל עוד הדרישות הנדרשות מראש מתקיימות, ניתן להפוך את Bitlocker "למצב הצפנה שקט" באמצעות המנגינה.</span><span class="sxs-lookup"><span data-stu-id="01878-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="01878-119">עיין בפרטים של דרישות ההתקן והגדרות מדיניות לדוגמה כדי לאפשר הצפנה שקטה במסמך הבא: [הפיכת הצפנת Bitlocker לזמינה בצורה שקטה](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="01878-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="01878-120">ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה ועוצמת הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="01878-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="01878-121">תשובה: לא.</span><span class="sxs-lookup"><span data-stu-id="01878-121">A: No.</span></span> <span data-ttu-id="01878-122">כדי להחיל את הגדרות הצופן החדשות, תחילה יש לפענח את הכונן.</span><span class="sxs-lookup"><span data-stu-id="01878-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="01878-123">**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכת מדיניות ההגדרה, המאפשרת שימוש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="01878-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="01878-124">ש: אם התקן מוצפן כתוצאה מתוך היישום של מדיניות ה-intune, האם היא תפענח כאשר מדיניות זו תוסר?</span><span class="sxs-lookup"><span data-stu-id="01878-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="01878-125">ת: הסרת מדיניות הקשורה להצפנה אינה מביאה לפענוח של הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="01878-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="01878-126">ש: מדוע מדיניות התאימות מציגה כי המכשיר שלי אינו מופעל על-ידי Bitlocker, למרות שהוא מופעל?</span><span class="sxs-lookup"><span data-stu-id="01878-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="01878-127">ת: ההגדרה "Bitlocker enabled" במדיניות התאימות של ' שימוש בעידון ' משתמשת בלקוח תקינות התקן של Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="01878-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="01878-128">לקוח זה מודד רק את מצב ההתקן בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="01878-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="01878-129">אז אם התקן לא אותחל מחדש מאז השלמת הצפנת Bitlocker, שירות הלקוח של DHA לא ידווח על Bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="01878-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 