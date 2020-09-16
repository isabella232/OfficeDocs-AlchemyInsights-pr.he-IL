---
title: עדכן את שרתי השמות כל שיצביעו על Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734912"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="87fa4-102">עדכן את שרתי השמות כל שיצביעו על Microsoft</span><span class="sxs-lookup"><span data-stu-id="87fa4-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="87fa4-103">הערה: הפצת השינויים בשרתי השמות עשויה להימשך עד 48 שעות.</span><span class="sxs-lookup"><span data-stu-id="87fa4-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="87fa4-104">כדי להגדיר את התחום שלך ב-Microsoft, יש לעדכן את nameservers אצל הרשם.</span><span class="sxs-lookup"><span data-stu-id="87fa4-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="87fa4-105">צור או ערוך את רשומות שרת השמות אצל רשם התחומים שלך.</span><span class="sxs-lookup"><span data-stu-id="87fa4-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="87fa4-106">עבור לאתר האינטרנט של רשם התחומים שלך וחפש את האזור שבו ניתן לערוך את שרתי השמות.</span><span class="sxs-lookup"><span data-stu-id="87fa4-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="87fa4-107">צור או ערוך שתי רשומות שרת שמות כך שיתאימו לערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="87fa4-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="87fa4-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="87fa4-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="87fa4-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="87fa4-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="87fa4-110">שמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="87fa4-110">Save changes.</span></span>

<span data-ttu-id="87fa4-111">באפשרותך גם למצוא הוראות מפורטות במאמר זה: [שינוי nameservers כדי להגדיר את Microsoft 365 עם רשם תחומים כלשהו](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="87fa4-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  