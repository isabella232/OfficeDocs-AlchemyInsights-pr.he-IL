---
title: עדכון שרתי השמות של התחום שלך ל- Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742179"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="0475d-102">עדכון שרתי השמות של התחום שלך ל- Office 365</span><span class="sxs-lookup"><span data-stu-id="0475d-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="0475d-103">הערה: הפצת השינויים בשרתי השמות עשויה להימשך עד 48 שעות.</span><span class="sxs-lookup"><span data-stu-id="0475d-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="0475d-p101">כדי להגדיר את התחום שלך ב- Office 365, ייתכן שיהיה עליך לעדכן את שרתי השמות אצל הרשם שלך. צור או ערוך את רשומות שרת השמות אצל רשם התחומים שלך.</span><span class="sxs-lookup"><span data-stu-id="0475d-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="0475d-106">עבור לאתר האינטרנט של רשם התחומים שלך וחפש את האזור שבו ניתן לערוך את שרתי השמות.</span><span class="sxs-lookup"><span data-stu-id="0475d-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="0475d-107">צור או ערוך שתי רשומות שרת שמות כך שיתאימו לערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0475d-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="0475d-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0475d-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="0475d-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0475d-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="0475d-110">שמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="0475d-110">Save changes.</span></span>

<span data-ttu-id="0475d-111">באפשרותך גם למצוא הוראות מפורטות במאמר זה: [שינוי שרתי שמות כדי להגדיר את Office 365 עם כל רשם תחומים](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="0475d-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  