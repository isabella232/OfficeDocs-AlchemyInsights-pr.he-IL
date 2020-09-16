---
title: מונחים חסרים במאגר המונחים של SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750452"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="bbef8-102">הפעלת הצפנת Bitlocker באמצעות ' כוונון '</span><span class="sxs-lookup"><span data-stu-id="bbef8-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="bbef8-103">ניתן להשתמש במדיניות הגנה מפני נקודות קצה כדי לקבוע את תצורת הגדרות ההצפנה של Boitlocker עבור מכשירי Windows כמתואר בהגדרות: Windows10 (ואילך) כדי להגן על מכשירים באמצעות ' כוונון '</span><span class="sxs-lookup"><span data-stu-id="bbef8-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="bbef8-104">עליך להיות מודע לכך שמכשירים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת bitlocker אוטומטית שמופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="bbef8-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="bbef8-105">פעולה זו עשויה להשפיע על יישום המדיניות אם תצורת הגדרות ברירת המחדל אינה מוגדרת.</span><span class="sxs-lookup"><span data-stu-id="bbef8-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="bbef8-106">ראה שאלות נפוצות לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="bbef8-106">See FAQ for more detail.</span></span>


<span data-ttu-id="bbef8-107"> שאלות נפוצות Q: אילו מהדורות של הצפנת מכשירים של Windows תומכת באמצעות מדיניות הגנה על נקודות קצה?</span><span class="sxs-lookup"><span data-stu-id="bbef8-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="bbef8-108"> ת: ההגדרות במדיניות הגנה על נקודות הקצה מתבצעות באמצעות CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="bbef8-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="bbef8-109">לא כל המהדורות או גירסאות build של Windows תומכות ב-CSP של Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="bbef8-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="bbef8-110">בשלב זה מהדורות Windows: Enterprise; התמיכה בחינוך, במכשירים ניידים, בארגונים ניידים ובמקצוענים (מגירסת build מס ' 1809 ואילך) נתמכת.</span><span class="sxs-lookup"><span data-stu-id="bbef8-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="bbef8-111">ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה ועוצמת הצופן (XTS-AES-128), החלת מדיניות באמצעות הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="bbef8-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="bbef8-112">תשובה: לא.</span><span class="sxs-lookup"><span data-stu-id="bbef8-112">A: No.</span></span> <span data-ttu-id="bbef8-113">כדי להחיל את הגדרות הצופן החדשות, יש לפענח תחילה את הכונן.</span><span class="sxs-lookup"><span data-stu-id="bbef8-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="bbef8-114">הערה עבור מכשירים שנרשמו באמצעות טייס אוטומטי ההצפנה האוטומטית שמתרחשת במהלך OOBE אינה מופעלת עד להערכת מדיניות ההגדרה המאפשרת להשתמש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה</span><span class="sxs-lookup"><span data-stu-id="bbef8-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="bbef8-115">ש אם התקן מוצפן כתוצאה מיישום מדיניות ה-intune, הוא יפוענח כאשר מדיניות זו תוסר?</span><span class="sxs-lookup"><span data-stu-id="bbef8-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="bbef8-116">ת: הסרת מדיניות קשורה להצפנה אינה מביאה לפענוח הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="bbef8-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="bbef8-117">ש: מדוע מדיניות התאימות מציגה כי ההתקן שלי אינו כולל את האפשרות ' מופעל ב-Bitlocker ' אך היא מתקיימת?</span><span class="sxs-lookup"><span data-stu-id="bbef8-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="bbef8-118">ת: ההגדרה ' מופעל ב-Bitlocker ' במדיניות תאימות של ' שימוש בעידון ' משתמשת בלקוח תקינות התקן של Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="bbef8-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="bbef8-119">לקוח זה מודד רק את מצב ההתקן בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="bbef8-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="bbef8-120">לכן, אם לא אותחל מכשיר מחדש מאז השלמת הצפנת bitlocker, שירות לקוח DHA לא ידווח על bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="bbef8-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>