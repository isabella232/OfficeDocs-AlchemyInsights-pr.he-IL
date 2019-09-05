---
title: התנאים החסרים בחנות המונח ' SharePoint Online '
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762063"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="fe1fb-102">הפעלת הצפנת Bitlocker עם Intune</span><span class="sxs-lookup"><span data-stu-id="fe1fb-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="fe1fb-103">ניתן להשתמש במדיניות הגנת נקודות קצה Intune כדי לקבוע את תצורת הגדרות ההצפנה של Boitlocker עבור התקני Windows כמתואר בהגדרות: Windows10 (ואילך) כדי להגן על התקנים באמצעות Intune</span><span class="sxs-lookup"><span data-stu-id="fe1fb-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="fe1fb-104">עליך להיות מודע לכך שהתקנים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת bitlocker אוטומטית המופעלת ללא היישום של מדיניות MDM.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="fe1fb-105">הדבר עלול להשפיע על יישום המדיניות אם לא נקבעה תצורה של הגדרות ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="fe1fb-106">לפרטים נוספים, ראה שאלות נפוצות.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-106">See FAQ for more detail.</span></span>


<span data-ttu-id="fe1fb-107">שאלות נפוצות  : אילו מהדורות של הצפנת התקן של Windows תומכות באמצעות מדיניות הגנת נקודות קצה?</span><span class="sxs-lookup"><span data-stu-id="fe1fb-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="fe1fb-108"> ת: ההגדרות במדיניות הגנת נקודות קצה Intune מיושמות באמצעות CSP של Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="fe1fb-109">לא כל המהדורות ובניית Windows תומכים ב-CSP של Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="fe1fb-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="fe1fb-110">בשלב זה Windows מהדורות: ארגון; השכלה, נייד, מפעל נייד ומקצועי (מ לבנות 1809 ואילך) נתמכים.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="fe1fb-111">ש: אם התקן מוצפן כבר באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה וחוזק הצופן (XTS-AES-128), תחיל מדיניות עם הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?</span><span class="sxs-lookup"><span data-stu-id="fe1fb-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="fe1fb-112">A: לא.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-112">A: No.</span></span> <span data-ttu-id="fe1fb-113">כדי להחיל את הגדרות ההצפנה החדשות, יש לפענח תחילה את הכונן.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="fe1fb-114">הערה עבור התקנים הרשומים עם טייס אוטומטי ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכה של מדיניות Intune המאפשרת להשתמש בהגדרות המבוססות על המדיניות במקום ברירות המחדל של מערכת ההפעלה</span><span class="sxs-lookup"><span data-stu-id="fe1fb-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="fe1fb-115">ש אם התקן מוצפן כתוצאה מיישום המדיניות הIntune האם הוא פוענח כאשר מדיניות זו תוסר?</span><span class="sxs-lookup"><span data-stu-id="fe1fb-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="fe1fb-116">ת: הסרת המדיניות הקשורה להצפנה אינה כתוצאה מפענוח הכוננים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="fe1fb-117">ש: מדוע מדיניות התאימות הintune מראה שלהתקן שלי אין "Bitlocker Enabled" אבל הוא?</span><span class="sxs-lookup"><span data-stu-id="fe1fb-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="fe1fb-118">ת: ההגדרה "Bitlocker enabled" במדיניות intune תאימות מנצלת את לקוח התקינות של Windows בריאות התקן (DHA).</span><span class="sxs-lookup"><span data-stu-id="fe1fb-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="fe1fb-119">לקוח זה מודד את מצב ההתקן בזמן האתחול.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="fe1fb-120">לכן, אם התקן לא אותחל מחודש מאז השלמת הצפנת bitlocker, שירות לקוח DHA לא ידווח על bitlocker כפעיל.</span><span class="sxs-lookup"><span data-stu-id="fe1fb-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>