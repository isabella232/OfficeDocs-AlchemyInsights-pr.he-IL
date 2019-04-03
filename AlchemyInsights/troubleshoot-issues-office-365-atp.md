---
title: פתרון בעיות עם Office 365 מתקדם איום הגנה (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030984"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="0d129-102">פתרון בעיות ב- Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="0d129-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="0d129-103">**שים לב עיכובים עם מסירת הודעות דואר אלקטרוני**?</span><span class="sxs-lookup"><span data-stu-id="0d129-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="0d129-104">נסה להשתמש באפשרות מסירה דינמי עבור פריטי מדיניות מסמכים מצורפים בטוחים של ATP.</span><span class="sxs-lookup"><span data-stu-id="0d129-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="0d129-105">כך יימנע עיכובים המסירה של הודעת דואר אלקטרוני תוך הגנה על נמענים מתוך קבצים מזיקים.</span><span class="sxs-lookup"><span data-stu-id="0d129-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="0d129-106">**ברצונך תוצאות false חיוביות הדוח או נגטיב שקר**?</span><span class="sxs-lookup"><span data-stu-id="0d129-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="0d129-107">השתמש בקישור זה כדי לשלוח את הקובץ עבור ניתוח:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="0d129-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="0d129-108">**ידעת כי באפשרותך להפעיל הגנה קישורים בטוח ATP עבור דואר אלקטרוני הנשלחות בין אנשים בארגון שלך**?</span><span class="sxs-lookup"><span data-stu-id="0d129-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="0d129-109">בצע שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="0d129-109">Follow these steps:</span></span>
    1. <span data-ttu-id="0d129-110">עבור אל https://protection.office.com, ולהיכנס.</span><span class="sxs-lookup"><span data-stu-id="0d129-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="0d129-111">עבור אל **ניהול איום** > **מדיניות** > **קישורים בטוח**.</span><span class="sxs-lookup"><span data-stu-id="0d129-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="0d129-112">תחת **מדיניות אשר חלים על נמענים ספציפיים**, לערוך (או להוסיף) מדיניות.</span><span class="sxs-lookup"><span data-stu-id="0d129-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="0d129-113">בחר **החל קישורים בטוח הודעות הנשלחות בתוך הארגון**.</span><span class="sxs-lookup"><span data-stu-id="0d129-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="0d129-114">שמירת מדיניות שלך ולאפשר שהשינויים שלך לעבודה שלהם דרך מרכז הנתונים שלך כ- 30 דקות.</span><span class="sxs-lookup"><span data-stu-id="0d129-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="0d129-115">כדי לקבל סיוע נוסף ATP, ראה [הגנה איום מתקדם של Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="0d129-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>