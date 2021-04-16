---
title: השתמש באפשרות ביטול נעילה של טביעת אצבע ב- Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796678"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="ec413-102">השתמש באפשרות ביטול נעילה של טביעת אצבע ב- Windows 10</span><span class="sxs-lookup"><span data-stu-id="ec413-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="ec413-103">**הפיכת טביעת אצבע של Windows Hello לזמינה**</span><span class="sxs-lookup"><span data-stu-id="ec413-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="ec413-104">כדי לבטל את נעילת Windows 10 באמצעות טביעת האצבע שלך, עליך להגדיר את Windows Hello Fingerprint על-ידי הוספה (מאפשרת ל- Windows ללמוד לזהות) לפחות אצבע אחת.</span><span class="sxs-lookup"><span data-stu-id="ec413-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="ec413-105">עבור אל **הגדרות > חשבונות > אפשרויות כניסה** (או לחץ [כאן](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="ec413-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="ec413-106">אפשרויות הכניסה הזמינות יופיעו ברשימה.</span><span class="sxs-lookup"><span data-stu-id="ec413-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="ec413-107">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="ec413-107">For example:</span></span>

    ![אפשרויות כניסה.](media/sign-in-options.png)

2. <span data-ttu-id="ec413-109">לחץ או הקש **על Windows Hello Fingerprint** ולאחר מכן לחץ על **הגדר**.</span><span class="sxs-lookup"><span data-stu-id="ec413-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="ec413-110">בחלון ההגדרה של Windows Hello, לחץ **על תחילת העבודה.**</span><span class="sxs-lookup"><span data-stu-id="ec413-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="ec413-111">חיישן טביעת האצבע יופעל, ותתבקש למקם את האצבע על החיישן:</span><span class="sxs-lookup"><span data-stu-id="ec413-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![חיישן טביעת אצבע.](media/fingerprint-sensor.png)

3. <span data-ttu-id="ec413-113">בצע את ההוראות, אשר יבקשו ממך לסרוק שוב ושוב את האצבע.</span><span class="sxs-lookup"><span data-stu-id="ec413-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="ec413-114">לאחר סיום פעולה זו, תהיה לך אפשרות להוסיף אצבעות אחרות שברצונך להשתמש עשויות להיות בשימוש עבור כניסה.</span><span class="sxs-lookup"><span data-stu-id="ec413-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="ec413-115">בפעם הבאה שת להיכנס ל- Windows 10, תהיה לך אפשרות להשתמש בטביעת האצבע שלך כדי לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="ec413-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="ec413-116">**טביעת אצבע של Windows Hello אינה זמינה כאפשרות כניסה**</span><span class="sxs-lookup"><span data-stu-id="ec413-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="ec413-117">אם טביעת אצבע של Windows Hello אינה מוצגת כאפשרות באפשרויות **כניסה,** פירוש הדבר ש- Windows אינו מודע לכל קורא טביעות אצבע/סורק המחובר למחשב שלך, או שמדיניות מערכת מונעת את השימוש בה (אם לדוגמה, המחשב שלך מנוהל על-ידי מקום העבודה שלך).</span><span class="sxs-lookup"><span data-stu-id="ec413-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="ec413-118">כדי לפתור בעיות:</span><span class="sxs-lookup"><span data-stu-id="ec413-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="ec413-119">בחר **בלחצן** התחל בשורת המשימות וחפש את **מנהל ההתקנים**.</span><span class="sxs-lookup"><span data-stu-id="ec413-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="ec413-120">לחץ או הקש כדי לפתוח את **מנהל ההתקנים**.</span><span class="sxs-lookup"><span data-stu-id="ec413-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="ec413-121">במנהל ההתקנים, הרחב את מכשירים ביומטריים על-ידי לחיצה על השבר השברולטי שלו.</span><span class="sxs-lookup"><span data-stu-id="ec413-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![מכשירים ביומטריים.](media/biometric-devices.png)

4. <span data-ttu-id="ec413-123">סורק טביעות האצבע שלך אמור להופיע כהתקן ביומטרי, כגון סורק WBDI של Synaptics:</span><span class="sxs-lookup"><span data-stu-id="ec413-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![מכשירים ביומטריים.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="ec413-125">אם סורק טביעות האצבע שלך אינו מוצג, והסורק משולב במחשב שלך, עבור אל אתר האינטרנט של יצרן המחשב.</span><span class="sxs-lookup"><span data-stu-id="ec413-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="ec413-126">במקטע התמיכה הטכנית של מודל המחשב שלך, חפש מנהל התקן של Windows 10 אחר סורק ש באפשרותך להתקין.</span><span class="sxs-lookup"><span data-stu-id="ec413-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="ec413-127">אם הסורק נפרד מהמחשב (מחובר באמצעות USB), עבור אל אתר האינטרנט של יצרן הסורק כדי למצוא ולהתקין את תוכנת מנהל ההתקן של Windows 10 עבור מודל הסורק שברשותך.</span><span class="sxs-lookup"><span data-stu-id="ec413-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
