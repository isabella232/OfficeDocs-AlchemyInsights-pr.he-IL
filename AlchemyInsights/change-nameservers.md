---
title: שינוי שרתי שמות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 148fbee1c14a8da6ede5ec5ccae90b1a4340ce32
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363078"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="086aa-102">עדכון שרתי השמות של התחום שלך ל- Office 365</span><span class="sxs-lookup"><span data-stu-id="086aa-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="086aa-103">הערה: הפצת השינויים בשרתי השמות עשויה להימשך עד 48 שעות.</span><span class="sxs-lookup"><span data-stu-id="086aa-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="086aa-p101">כדי להגדיר את התחום שלך ב- Office 365, ייתכן שיהיה עליך לעדכן את שרתי השמות אצל הרשם שלך. צור או ערוך את רשומות שרת השמות אצל רשם התחומים שלך.</span><span class="sxs-lookup"><span data-stu-id="086aa-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="086aa-106">עבור לאתר האינטרנט של רשם התחומים שלך וחפש את האזור שבו ניתן לערוך את שרתי השמות.</span><span class="sxs-lookup"><span data-stu-id="086aa-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="086aa-107">צור או ערוך שתי רשומות שרת שמות כך שיתאימו לערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="086aa-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="086aa-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="086aa-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="086aa-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="086aa-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="086aa-110">שמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="086aa-110">Save changes.</span></span>

<span data-ttu-id="086aa-111">באפשרותך גם למצוא הוראות מפורטות במאמר זה: [שינוי שרתי שמות כדי להגדיר את Office 365 עם כל רשם תחומים](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="086aa-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  