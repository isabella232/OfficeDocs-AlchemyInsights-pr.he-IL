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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219856"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="85047-102">חסימה או ביטול חסימה של העברת דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="85047-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="85047-103">כדי להפוך העברת דואר אלקטרוני לזמינה או ללא זמינה עבור תיבת דואר ספציפית, ראה [קביעת תצורה של העברת דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="85047-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="85047-104">ברמת הדיירים, השליטה על העברה חיצונית מתבצעת באמצעות המדיניות היוצאת למניעת דואר זבל.</span><span class="sxs-lookup"><span data-stu-id="85047-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="85047-105">אם הוא מוגדר כבוטל או אוטומטי, ייתכן שהוא יחסום את העברת הדואר האלקטרוני באמצעות השגיאה "550 5.7.520 הגישה נדחתה, הארגון שלך אינו מאפשר העברה חיצונית".</span><span class="sxs-lookup"><span data-stu-id="85047-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="85047-106">לאחר מכן, אם הוגדרה העברה שנחסמה, זוהי השגיאה שהמשתמשים יראו.</span><span class="sxs-lookup"><span data-stu-id="85047-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="85047-107">אם העברת העברה נחסמת, ודא שהמדיניות נקבעה להפיכת Autoforward חיצוניים לזמין.</span><span class="sxs-lookup"><span data-stu-id="85047-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="85047-108">באפשרותך לבדוק את מדיניות המסנן ' דואר זבל יוצא ' ממרכז האבטחה והתאימות או על-ידי הפעלת Get-HostedOutboundSpamFilterPolicy | שם fl, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="85047-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="85047-109">אם ברצונך להגדיר חסימת Autoforward, אותה פקודה תספר לך את מצב המדיניות כעת.</span><span class="sxs-lookup"><span data-stu-id="85047-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="85047-110">הערה: מומלץ להשאיר את הAutoforward החיצוניים ללא זמין במדיניות מסנן דואר הזבל היוצא המהווה ברירת מחדל ולהפוך אותה לזמינה רק עבור המשתמשים הזקוקים להעברה חיצונית על-ידי יצירת מדיניות מותאמת אישית עבור משתמשים אלה.</span><span class="sxs-lookup"><span data-stu-id="85047-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="85047-111">באפשרותך לקרוא עוד [בקביעת התצורה של העברת דואר אלקטרוני חיצוני ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="85047-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>