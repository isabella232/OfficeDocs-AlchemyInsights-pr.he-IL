---
title: שינוי שרתי שמות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818613"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="00004-102">עדכן את שרתי השמות כל שיצביעו על Microsoft</span><span class="sxs-lookup"><span data-stu-id="00004-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="00004-103">הערה: הפצת השינויים בשרתי השמות עשויה להימשך עד 48 שעות.</span><span class="sxs-lookup"><span data-stu-id="00004-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="00004-p101">כדי להגדיר את התחום שלך ב- Microsoft 365, ייתכן שיהיה עליך לעדכן את שרתי השמות אצל הרשם שלך. צור או ערוך את רשומות שרת השמות אצל רשם התחומים שלך.</span><span class="sxs-lookup"><span data-stu-id="00004-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="00004-106">עבור לאתר האינטרנט של רשם התחומים שלך וחפש את האזור שבו ניתן לערוך את שרתי השמות.</span><span class="sxs-lookup"><span data-stu-id="00004-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="00004-107">צור או ערוך שתי רשומות שרת שמות כך שיתאימו לערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="00004-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="00004-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="00004-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="00004-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="00004-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="00004-110">שמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="00004-110">Save changes.</span></span>

<span data-ttu-id="00004-111">באפשרותך גם למצוא הוראות מפורטות במאמר זה: [שינוי שרתי שמות עם כל רשם תחומים](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="00004-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  