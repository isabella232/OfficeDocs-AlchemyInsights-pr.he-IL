---
title: שינוי שרתי שמות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706756"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="32deb-102">עדכן את שרתי השמות כל שיצביעו על Microsoft</span><span class="sxs-lookup"><span data-stu-id="32deb-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="32deb-103">הערה: הפצת השינויים בשרתי השמות עשויה להימשך עד 48 שעות.</span><span class="sxs-lookup"><span data-stu-id="32deb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="32deb-p101">כדי להגדיר את התחום שלך ב- Microsoft 365, ייתכן שיהיה עליך לעדכן את שרתי השמות אצל הרשם שלך. צור או ערוך את רשומות שרת השמות אצל רשם התחומים שלך.</span><span class="sxs-lookup"><span data-stu-id="32deb-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="32deb-106">עבור לאתר האינטרנט של רשם התחומים שלך וחפש את האזור שבו ניתן לערוך את שרתי השמות.</span><span class="sxs-lookup"><span data-stu-id="32deb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="32deb-107">צור או ערוך שתי רשומות שרת שמות כך שיתאימו לערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="32deb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="32deb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="32deb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="32deb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="32deb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="32deb-110">שמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="32deb-110">Save changes.</span></span>

<span data-ttu-id="32deb-111">באפשרותך גם למצוא הוראות מפורטות במאמר זה: [שינוי שרתי שמות עם כל רשם תחומים](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="32deb-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  