---
title: פתרון בעיות עם הגנת האיום המתקדם של Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511113"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="93008-102">פתרון בעיות באמצעות Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="93008-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="93008-103">**הודעה על עיכובים במסירת הודעת דואר אלקטרוני**?</span><span class="sxs-lookup"><span data-stu-id="93008-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="93008-104">נסה להשתמש באפשרות ' מסירה דינאמית ' עבור מדיניות הקבצים המצורפים של ATP.</span><span class="sxs-lookup"><span data-stu-id="93008-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="93008-105">פעולה זו תמנע עיכובים בהעברת הודעות דואר אלקטרוני תוך הגנה על נמענים מפני קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="93008-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="93008-106">**האם ברצונך לדווח על תוצאות חיוביות שגויות או על שליליות שווא**?</span><span class="sxs-lookup"><span data-stu-id="93008-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="93008-107">השתמש בקישור זה כדי לשלוח את הקובץ לניתוח:https://microsoft.com/wdsi/filesubmission</span><span class="sxs-lookup"><span data-stu-id="93008-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="93008-108">**האם ידעת שבאפשרותך לאפשר הגנה מפני קישורים בטוחים של ATP עבור דואר אלקטרוני שנשלח בין אנשים בארגון שלך**?</span><span class="sxs-lookup"><span data-stu-id="93008-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="93008-109">בצע שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="93008-109">Follow these steps:</span></span>
    1. <span data-ttu-id="93008-110">. קדימה https://protection.office.com , ותחתמי</span><span class="sxs-lookup"><span data-stu-id="93008-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="93008-111">עבור אל מדיניות **ניהול האיום**  >  **Policy**  >  **קישורים בטוחים**.</span><span class="sxs-lookup"><span data-stu-id="93008-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="93008-112">תחת **פריטי מדיניות החלים על נמענים ספציפיים**, ערוך (או הוסף) מדיניות.</span><span class="sxs-lookup"><span data-stu-id="93008-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="93008-113">בחר באפשרות **החל קישורים בטוחים על הודעות הנשלחות בתוך הארגון**.</span><span class="sxs-lookup"><span data-stu-id="93008-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="93008-114">שמור את המדיניות שלך והמתן 30 דקות לשינויים שביצעת כדי לעבוד דרך מרכז הנתונים.</span><span class="sxs-lookup"><span data-stu-id="93008-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="93008-115">כדי לקבל עזרה נוספת ב-ATP, ראה [הגנת האיום המתקדמת של Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="93008-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>