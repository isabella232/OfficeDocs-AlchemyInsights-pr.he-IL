---
title: הפיכת ביקורת תיבת דואר לזמינה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814193"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="54d4b-102">הפיכת ביקורת תיבת דואר לזמינה</span><span class="sxs-lookup"><span data-stu-id="54d4b-102">Enable mailbox auditing</span></span>

<span data-ttu-id="54d4b-103">כדי להפוך ביקורת תיבות דואר לזמינה עבור משתמש יחיד או ארגון שלם, יש להפעיל את כלי ה- cmdlet הבאים מתוך מעטפת Power Remote:</span><span class="sxs-lookup"><span data-stu-id="54d4b-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="54d4b-104">**משתמש יחיד**</span><span class="sxs-lookup"><span data-stu-id="54d4b-104">**Single User**</span></span>
  
<span data-ttu-id="54d4b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="54d4b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="54d4b-106">**ארגון**</span><span class="sxs-lookup"><span data-stu-id="54d4b-106">**Organization**</span></span>
  
<span data-ttu-id="54d4b-107">Get-Mailbox-ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="54d4b-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="54d4b-108">למד עוד</span><span class="sxs-lookup"><span data-stu-id="54d4b-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

