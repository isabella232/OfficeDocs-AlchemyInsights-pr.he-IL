---
title: שימוש באפשרות נעילת טביעת אצבע ב-Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795245"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="d73d9-102">שימוש באפשרות נעילת טביעת אצבע ב-Windows 10</span><span class="sxs-lookup"><span data-stu-id="d73d9-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="d73d9-103">**הפיכת טביעת אצבע של Windows לזמינה**</span><span class="sxs-lookup"><span data-stu-id="d73d9-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="d73d9-104">כדי לבטל את הנעילה של Windows 10 באמצעות טביעת האצבע שלך, עליך להגדיר טביעת אצבע של Windows על-ידי הוספה (המאפשר ל-Windows ללמוד לזהות) לפחות אצבע אחת.</span><span class="sxs-lookup"><span data-stu-id="d73d9-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="d73d9-105">עבור אל **הגדרות חשבונות > > אפשרויות כניסה** (או לחץ [כאן](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="d73d9-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d73d9-106">אפשרויות כניסה זמינות יופיעו.</span><span class="sxs-lookup"><span data-stu-id="d73d9-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="d73d9-107">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="d73d9-107">For example:</span></span>

    ![אפשרויות כניסה.](media/sign-in-options.png)

2. <span data-ttu-id="d73d9-109">לחץ או הקש על **טביעת אצבע של Windows שלום**ולאחר מכן לחץ על **הגדר**.</span><span class="sxs-lookup"><span data-stu-id="d73d9-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="d73d9-110">בחלון הגדרת שלום של Windows, לחץ על **תחילת**העבודה.</span><span class="sxs-lookup"><span data-stu-id="d73d9-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="d73d9-111">חיישן טביעות האצבע יופעל, ותתבקש למקם את האצבע על החיישן:</span><span class="sxs-lookup"><span data-stu-id="d73d9-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![חיישן טביעות אצבעות.](media/fingerprint-sensor.png)

3. <span data-ttu-id="d73d9-113">בצע את ההוראות, אשר יבקש ממך לסרוק שוב ושוב את האצבע.</span><span class="sxs-lookup"><span data-stu-id="d73d9-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="d73d9-114">כאשר פעולה זו תסתיים, תהיה לך אפשרות להוסיף אצבעות אחרות שייתכן שתרצה להשתמש בהן לכניסה.</span><span class="sxs-lookup"><span data-stu-id="d73d9-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="d73d9-115">בפעם הבאה שתיכנס ל-Windows 10, תהיה לך אפשרות להשתמש בטביעת האצבע כדי לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="d73d9-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="d73d9-116">**טביעת אצבע של Windows שלום אינה זמינה כאפשרות כניסה**</span><span class="sxs-lookup"><span data-stu-id="d73d9-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="d73d9-117">אם טביעת האצבע של Windows שלום אינה מוצגת כאפשרות **באפשרויות כניסה**, משמעות הדבר היא ש-windows אינו מודע לקורא או לסורק טביעות האצבע המצורפים למחשב שלך, או שמדיניות מערכת מונעת את השימוש בה (אם למשל המחשב שלך מנוהל על-ידי מקום העבודה שלך).</span><span class="sxs-lookup"><span data-stu-id="d73d9-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="d73d9-118">כדי לפתור בעיות:</span><span class="sxs-lookup"><span data-stu-id="d73d9-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="d73d9-119">בחר את לחצן **התחל** בשורת המשימות וחפש את **מנהל ההתקנים**.</span><span class="sxs-lookup"><span data-stu-id="d73d9-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="d73d9-120">לחץ או הקש כדי לפתוח את **מנהל ההתקנים**.</span><span class="sxs-lookup"><span data-stu-id="d73d9-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="d73d9-121">במנהל ההתקנים, הרחב את המכשירים הביומטריים על-ידי לחיצה על סוגר הזוויתי</span><span class="sxs-lookup"><span data-stu-id="d73d9-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![מכשירים ביומטריים.](media/biometric-devices.png)

4. <span data-ttu-id="d73d9-123">סורק טביעות האצבע אמור להופיע כהתקן ביומטרי, כגון הסורק Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="d73d9-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![מכשירים ביומטריים.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="d73d9-125">אם סורק טביעות האצבע שלך אינו מוצג, והסורק משולב במחשב שלך, עבור אל אתר האינטרנט של יצרן המחשב.</span><span class="sxs-lookup"><span data-stu-id="d73d9-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="d73d9-126">במקטע תמיכה טכנית עבור מודל PC שלך, חפש מנהל התקן של Windows 10 עבור סורק שניתן להתקין.</span><span class="sxs-lookup"><span data-stu-id="d73d9-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="d73d9-127">אם הסורק נפרד מהמחשב (מחובר באמצעות USB), עבור אל אתר האינטרנט של יצרן הסורק כדי לחפש ולהתקין את תוכנת מנהל ההתקן של Windows 10 עבור מודל הסורק שברשותך.</span><span class="sxs-lookup"><span data-stu-id="d73d9-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
