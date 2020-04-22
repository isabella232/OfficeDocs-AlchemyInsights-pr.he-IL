---
title: הפיכת ביקורת תיבת דואר לזמינה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703572"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="562db-102">הפיכת ביקורת תיבת דואר לזמינה</span><span class="sxs-lookup"><span data-stu-id="562db-102">Enable mailbox auditing</span></span>

<span data-ttu-id="562db-103">כדי להפעיל את ביקורת תיבת הדואר עבור משתמש יחיד או ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים ממעטפת החשמל המרוחקת:</span><span class="sxs-lookup"><span data-stu-id="562db-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="562db-104">**משתמש יחיד**</span><span class="sxs-lookup"><span data-stu-id="562db-104">**Single User**</span></span>
  
<span data-ttu-id="562db-105">הגדר-תיבת דואר-זהות "ג ' יין דאו"-מ$true השמע</span><span class="sxs-lookup"><span data-stu-id="562db-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="562db-106">**ארגון**</span><span class="sxs-lookup"><span data-stu-id="562db-106">**Organization**</span></span>
  
<span data-ttu-id="562db-107">קבל-תיבת דואר-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | הגדרת מ$true באמצעות תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="562db-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="562db-108">למד עוד</span><span class="sxs-lookup"><span data-stu-id="562db-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

