---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815616"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="7e442-102">הפיכת הצפנת Bitlocker לזמין באמצעות Intune</span><span class="sxs-lookup"><span data-stu-id="7e442-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="7e442-103">ניתן להשתמש במדיניות הגנת קצה של Intune כדי לקבוע את התצורה של הגדרות ההצפנה של Bitlocker עבור מכשירי Windows.</span><span class="sxs-lookup"><span data-stu-id="7e442-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="7e442-104">לקבלת מידע נוסף, ראה [הגדרות Windows 10 (ואילך) כדי להגן על מכשירים באמצעות Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="7e442-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="7e442-105">בנוסף למדיניות ההגנה על נקודות הקצה, ישנו גם דוח הצפנה המספק תצוגה מפורטת יותר של מצב ההצפנה עבור מכשירים.</span><span class="sxs-lookup"><span data-stu-id="7e442-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="7e442-106">ניתן לגשת הדוח זה בפורטל MEM תחת מכשירים **> צג** ולאחר מכן, תחת קביעת **תצורה,** [בחר הצפנה הדוח](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span><span class="sxs-lookup"><span data-stu-id="7e442-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="7e442-107">אם אתה מוצא ש- Bitlocker אינו זמין כצפוי או שהפרופיל המשמש לזמינה של Bitlocker נמצא במצב שגיאה, עיין בהצפנה הדוח כדי להבין טוב יותר מדוע מתרחש אופן הפעולה.</span><span class="sxs-lookup"><span data-stu-id="7e442-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="7e442-108">כדי למצוא פרטים לגבי האופן שבו ניתן לפרש את הדוח, כולל ערכי מצב ההצפנה השונים, ראה [ניטור הצפנת מכשיר באמצעות Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span><span class="sxs-lookup"><span data-stu-id="7e442-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="7e442-109">עליך להיות מודע לכך שהתקנים חדשים רבים פועלים עם Windows 10 תומכים בהצפנה אוטומטית של Bitlocker, המופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="7e442-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="7e442-110">פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן מוגדרות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="7e442-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="7e442-111">לקבלת פרטים נוספים, עיין בשאלות הנפוצות הבאות.</span><span class="sxs-lookup"><span data-stu-id="7e442-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="7e442-112">לקבלת מידע אודות פתרון בעיות ב- bitlocker, ראה [פתרון בעיות של פריטי מדיניות של BitLocker ב- Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="7e442-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="7e442-113">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="7e442-113">**FAQ**</span></span>

<span data-ttu-id="7e442-114">ש: אילו מהדורות של הצפנת התקן של Windows תומכות באמצעות מדיניות ההגנה על נקודות הקצה?</span><span class="sxs-lookup"><span data-stu-id="7e442-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="7e442-115">ת: ההגדרות במדיניות הגנת קצה של Intune מיושמות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="7e442-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="7e442-116">לא כל המהדורות או הגרסאות build של Windows תומכות ב- CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="7e442-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="7e442-117">ש: כיצד ניתן להפוך את Bitlocker לזמין במכשירים ללא צורך באינטראקציה של משתמש קצה?</span><span class="sxs-lookup"><span data-stu-id="7e442-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="7e442-118">ת: כל עוד התנאים המוקדמים הדרושים יתקינו, ניתן להפוך את Bitlocker לזמין "הצפנה שקטה" באמצעות Intune.</span><span class="sxs-lookup"><span data-stu-id="7e442-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="7e442-119">עיין בפרטים של דרישות המכשיר והגדרות מדיניות לדוגמה כדי להפוך הצפנה שקטה לזמינה במסמך הבא: [שקט הפוך הצפנת Bitlocker לזמינה.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)</span><span class="sxs-lookup"><span data-stu-id="7e442-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="7e442-120">ש: אם מכשיר כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת הצפנה וחוזק הצפנה (XTS-AES-128), החלת מדיניות עם הגדרות שונות מפעילה באופן אוטומטי הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="7e442-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="7e442-121">תשובה: לא.</span><span class="sxs-lookup"><span data-stu-id="7e442-121">A: No.</span></span> <span data-ttu-id="7e442-122">כדי להחיל את הגדרות הצופן החדשות, יש לפענח תחילה את הכונן.</span><span class="sxs-lookup"><span data-stu-id="7e442-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="7e442-123">**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שמתרחשת במהלך OOBE אינה מופעלת עד להערכה של מדיניות Intune, המאפשרת להשתמש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="7e442-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="7e442-124">ש: אם מכשיר מוצפן כתוצאה מיישום מדיניות Intune, האם הוא יפענח בעת הסרת מדיניות זו?</span><span class="sxs-lookup"><span data-stu-id="7e442-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="7e442-125">ת: הסרת מדיניות הקשורה להצפנה אינה כוללת פענוח של הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="7e442-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="7e442-126">ש: מדוע מדיניות תאימות Intune מראה שהמכשיר שלי אינו זמין ב- Bitlocker, למרות שהוא זמין?</span><span class="sxs-lookup"><span data-stu-id="7e442-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="7e442-127">ת: ההגדרה "Bitlocker enabled" במדיניות תאימות Intune משתמשת בלקוח בדיקת תקינות התקן Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="7e442-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="7e442-128">לקוח זה מודד את מצב המכשיר רק בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="7e442-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="7e442-129">לכן, אם לא אותחל מחדש מכשיר מאז השלמת ההצפנה של Bitlocker, שירות לקוח DHA לא הדוח Bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="7e442-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 