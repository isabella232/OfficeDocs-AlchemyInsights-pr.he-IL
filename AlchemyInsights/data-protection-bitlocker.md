---
title: הגנת נתונים-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908711"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5cf60-102">הפעלת הצפנת Bitlocker עם Intune</span><span class="sxs-lookup"><span data-stu-id="5cf60-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="5cf60-103">ניתן להשתמש במדיניות הגנת נקודות קצה Intune כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור התקני Windows.</span><span class="sxs-lookup"><span data-stu-id="5cf60-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="5cf60-104">לקבלת מידע נוסף, ראה [הגדרות Windows 10 (וגירסאות מאוחרות יותר) כדי להגן על התקנים באמצעות Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="5cf60-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="5cf60-105">עליך להיות מודע לכך שהתקנים חדשים רבים בהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, המופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="5cf60-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5cf60-106">הדבר עלול להשפיע על יישום המדיניות אם תצורתה של הגדרות שאינן מוגדרות כברירת מחדל נקבעה.</span><span class="sxs-lookup"><span data-stu-id="5cf60-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="5cf60-107">לפרטים נוספים, עיין בשאלות הנפוצות הבאות.</span><span class="sxs-lookup"><span data-stu-id="5cf60-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="5cf60-108">לקבלת מידע אודות פתרון בעיות [באמצעות bitlocker, ראה פתרון בעיות של מדיניות bitlocker ב-Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="5cf60-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="5cf60-109">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="5cf60-109">**FAQ**</span></span>

 <span data-ttu-id="5cf60-110">ש: אילו מהדורות של הצפנת התקן של Windows תומכות באמצעות מדיניות הגנת נקודות קצה?</span><span class="sxs-lookup"><span data-stu-id="5cf60-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="5cf60-111">ת: ההגדרות במדיניות הגנת נקודות קצה Intune מיושמות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="5cf60-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="5cf60-112">לא כל המהדורות או בניית Windows תומכים ב-CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="5cf60-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="5cf60-113">בשלב זה, המהדורות הבאות של Windows נתמכות: ארגון, חינוך, נייד, מפעל נייד ומקצועי (לבנות 1809 ומעלה).</span><span class="sxs-lookup"><span data-stu-id="5cf60-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="5cf60-114">ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה וחוזק הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות תפעיל באופן אוטומטי הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="5cf60-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="5cf60-115">A: לא.</span><span class="sxs-lookup"><span data-stu-id="5cf60-115">A: No.</span></span> <span data-ttu-id="5cf60-116">כדי להחיל את הגדרות ההצפנה החדשות, יש לפענח תחילה את הכונן.</span><span class="sxs-lookup"><span data-stu-id="5cf60-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="5cf60-117">**הערה:** עבור התקנים הרשומים עם טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכה של מדיניות Intune, דבר המאפשר להשתמש בהגדרות מבוססות המדיניות במקום ברירות המחדל של מערכת ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="5cf60-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="5cf60-118">ש: אם התקן מוצפן כתוצאה מיישום מדיניות Intune, האם הוא יהיה מפוענח בעת הסרת מדיניות זו?</span><span class="sxs-lookup"><span data-stu-id="5cf60-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="5cf60-119">ת: הסרת מדיניות הקשורה להצפנה אינה נובעת מפענוח הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="5cf60-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="5cf60-120">ש: מדוע מדיניות התאימות של Intune מראה שלהתקן שלי אין Bitlocker מאופשר, למרות שהוא?</span><span class="sxs-lookup"><span data-stu-id="5cf60-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="5cf60-121">ת: ההגדרה "Bitlocker מאופשר" במדיניות התאימות Intune מנצלת את לקוח בריאות ההתקנים של Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="5cf60-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5cf60-122">לקוח זה מודד את מצב ההתקן בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="5cf60-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="5cf60-123">לכן, אם התקן לא אותחל מההתחלה מאחר שהצפנת Bitlocker הושלמה, שירות לקוח DHA לא ידווח על Bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="5cf60-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 