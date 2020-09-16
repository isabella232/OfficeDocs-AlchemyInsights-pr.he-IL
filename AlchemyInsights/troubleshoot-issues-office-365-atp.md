---
title: פתרון בעיות בנושא הגנת האיום המתקדמת של Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758066"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="ea23f-102">פתרון בעיות באמצעות Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="ea23f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="ea23f-103">**העברת הודעות באמצעות העברת הודעות דואר אלקטרוני**?</span><span class="sxs-lookup"><span data-stu-id="ea23f-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="ea23f-104">נסה להשתמש באפשרות המסירה הדינאמית עבור מדיניות הקבצים המצורפים הבטוחים של ATP.</span><span class="sxs-lookup"><span data-stu-id="ea23f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="ea23f-105">פעולה זו תמנע עיכובים במסירת הודעות דואר אלקטרוני תוך הגנה על נמענים מקבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="ea23f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="ea23f-106">**האם ברצונך לדווח על חיובים שקריים או על נגטיב שווא**?</span><span class="sxs-lookup"><span data-stu-id="ea23f-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="ea23f-107">השתמש בקישור זה כדי לשלוח את הקובץ לניתוח: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="ea23f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="ea23f-108">**האם ידעת שניתן להפעיל הגנה על קישורים בטוחים של ATP עבור דואר אלקטרוני שנשלח בין אנשים בארגון שלך**?</span><span class="sxs-lookup"><span data-stu-id="ea23f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="ea23f-109">בצע שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="ea23f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="ea23f-110">עבור אל https://protection.office.com והיכנס.</span><span class="sxs-lookup"><span data-stu-id="ea23f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="ea23f-111">עבור אל **Threat management**  >  קישורים בטוחים**של מדיניות**ניהול איום  >  **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="ea23f-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="ea23f-112">תחת **פריטי מדיניות החלים על נמענים ספציפיים**, ערוך (או הוסף) מדיניות.</span><span class="sxs-lookup"><span data-stu-id="ea23f-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="ea23f-113">בחר באפשרות **החל קישורים בטוחים על הודעות הנשלחות בתוך הארגון**.</span><span class="sxs-lookup"><span data-stu-id="ea23f-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="ea23f-114">שמור את המדיניות, והמתן כ-30 דקות כדי שהשינויים יתבצעו דרך מרכז הנתונים שלך.</span><span class="sxs-lookup"><span data-stu-id="ea23f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="ea23f-115">כדי לקבל עזרה נוספת עם ATP, ראה [הגנת האיום המתקדמת של Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="ea23f-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>