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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506955"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="f0c61-102">הפיכת ביקורת תיבת דואר לזמינה</span><span class="sxs-lookup"><span data-stu-id="f0c61-102">Enable mailbox auditing</span></span>

<span data-ttu-id="f0c61-103">כדי להפעיל את ביקורת תיבת הדואר עבור משתמש יחיד או ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים ממעטפת החשמל המרוחקת:</span><span class="sxs-lookup"><span data-stu-id="f0c61-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="f0c61-104">**משתמש יחיד**</span><span class="sxs-lookup"><span data-stu-id="f0c61-104">**Single User**</span></span>
  
<span data-ttu-id="f0c61-105">הגדר-תיבת דואר-זהות "ג ' יין דאו"-מ$true השמע</span><span class="sxs-lookup"><span data-stu-id="f0c61-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="f0c61-106">**ארגון**</span><span class="sxs-lookup"><span data-stu-id="f0c61-106">**Organization**</span></span>
  
<span data-ttu-id="f0c61-107">קבל-תיבת דואר-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | הגדרת מ$true באמצעות תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="f0c61-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="f0c61-108">למד עוד</span><span class="sxs-lookup"><span data-stu-id="f0c61-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

