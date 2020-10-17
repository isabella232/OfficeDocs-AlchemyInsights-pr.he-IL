---
title: 726 חסימת העברת דואר אלקטרוני
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478340"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="19498-102">חסימה או ביטול חסימה של העברת דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="19498-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="19498-103">כדי להפוך העברת דואר אלקטרוני לזמינה או ללא זמינה עבור תיבת דואר ספציפית, ראה [קביעת תצורה של העברת דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="19498-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="19498-104">ברמת הדייר, השליטה על העברה חיצונית מתבצעת באמצעות מדיניות הדואר האלקטרוני היוצא.</span><span class="sxs-lookup"><span data-stu-id="19498-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="19498-105">באפשרותך לבדוק את מדיניות המסנן של דואר זבל יוצא ממרכז האבטחה והתאימות [כאן](https://protection.office.com/antispam) או באמצעות [הפקודה Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="19498-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="19498-106">אם אתה מקבל את השגיאה הבאה: **"550 5.7.520 Access נדחה, הארגון שלך אינו מאפשר העברה חיצונית"**, ודא שהמדיניות מוגדרת להפיכת העברה אוטומטית אוטומטית לזמינה.</span><span class="sxs-lookup"><span data-stu-id="19498-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="19498-107">**הערה:** מומלץ למנוע מAutoforward החיצוניות להיות זמין במדיניות מסנן דואר הזבל היוצא המהווה ברירת מחדל, ולהפוך אותה לזמינה רק עבור המשתמשים הזקוקים להעברה חיצונית על-ידי יצירת מדיניות מותאמת אישית עבור משתמשים אלה.</span><span class="sxs-lookup"><span data-stu-id="19498-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="19498-108">באפשרותך לקרוא עוד [בקביעת התצורה של העברת דואר אלקטרוני חיצוני ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="19498-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>