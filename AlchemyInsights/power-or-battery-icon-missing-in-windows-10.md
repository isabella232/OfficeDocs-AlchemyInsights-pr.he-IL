---
title: סמל הסוללה או החשמל חסר ב- Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790549"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="f9c00-102">סמל הסוללה או החשמל חסר ב- Windows 10</span><span class="sxs-lookup"><span data-stu-id="f9c00-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="f9c00-103">אם במכשיר Windows 10 יש סוללה (לדוגמה, מחשב נישא או טאבלט או מחשב PC המחובר באמצעות USB ל- UPS), סמל מצב החשמל/סוללה מוצג בדרך כלל בשורת המשימות ליד השעון, לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="f9c00-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![סמל הסוללה](media/battery-icon.png)

<span data-ttu-id="f9c00-105">אם אינך רואה את הסמל, ייתכן שהוא מוסתר:</span><span class="sxs-lookup"><span data-stu-id="f9c00-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="f9c00-106">עבור אל **[ההגדרות > התאמה אישית > שורת המשימות](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="f9c00-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="f9c00-107">באזור ההודעות, לחץ על **בחר אילו סמלים יופיעו בשורת המשימות**.</span><span class="sxs-lookup"><span data-stu-id="f9c00-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="f9c00-108">לאחר מכן, מצא את פריט ה **חשמל** ברשימה והחלף את ההגדרה שלו ל- **פועל**.</span><span class="sxs-lookup"><span data-stu-id="f9c00-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![הצגת סמל החשמל בשורת המשימות](media/power-icon-on.png)

<span data-ttu-id="f9c00-110">**פתרון בעיות**</span><span class="sxs-lookup"><span data-stu-id="f9c00-110">**Troubleshooting**</span></span>

<span data-ttu-id="f9c00-111">אם ההוראות שלעיל והלחצן הדו-מצבי **חשמל** מופיע באפור או אינו גלוי, בתיבת החיפוש בשורת המשימות, הקלד **מנהל ההתקנים** ולאחר מכן בחר **מנהל ההתקנים** ברשימת התוצאות.</span><span class="sxs-lookup"><span data-stu-id="f9c00-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="f9c00-112">באזור **סוללות**, לחץ באמצעות לחצן העכבר הימני על הסוללה עבור המכשיר שלך, לחץ על **הפוך ללא זמין** ולאחר מכן לחץ על **כן**.</span><span class="sxs-lookup"><span data-stu-id="f9c00-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="f9c00-113">המתן כמה שניות ולאחר מכן לחץ באמצעות לחצן העכבר הימני על הסוללה ולחץ על **הפוך לזמין**.</span><span class="sxs-lookup"><span data-stu-id="f9c00-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="f9c00-114">לאחר מכן הפעל מחדש את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="f9c00-114">Then restart your device.</span></span>

<span data-ttu-id="f9c00-115">אם בצעת את ההוראות לעיל, אך סמל הסוללה לא מופיע בשורת המשימות, בתיבת החיפוש בשורת המשימות, הקלד **מנהל המשימות** ולאחר מכן לחץ על **מנהל המשימות** ברשימת התוצאות.</span><span class="sxs-lookup"><span data-stu-id="f9c00-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="f9c00-116">בכרטיסיה **תהליכים**, תחת **שם**, לחץ באמצעות לחצן העכבר הימני על **Explorer** ולאחר מכן לחץ על **הפעל מחדש**.</span><span class="sxs-lookup"><span data-stu-id="f9c00-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
