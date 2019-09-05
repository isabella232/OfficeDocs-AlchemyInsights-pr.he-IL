---
title: הפיכת ביקורת תיבת דואר לזמינה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736254"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="6acf0-102">הפיכת ביקורת תיבת דואר לזמינה</span><span class="sxs-lookup"><span data-stu-id="6acf0-102">Enable mailbox auditing</span></span>

<span data-ttu-id="6acf0-103">כדי להפעיל את ביקורת תיבת הדואר עבור משתמש יחיד או ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים ממעטפת החשמל המרוחקת:</span><span class="sxs-lookup"><span data-stu-id="6acf0-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="6acf0-104">**משתמש יחיד**</span><span class="sxs-lookup"><span data-stu-id="6acf0-104">**Single User**</span></span>
  
<span data-ttu-id="6acf0-105">הגדר-תיבת דואר-זהות "ג ' יין דאו"-מ$true השמע</span><span class="sxs-lookup"><span data-stu-id="6acf0-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="6acf0-106">**ארגון**</span><span class="sxs-lookup"><span data-stu-id="6acf0-106">**Organization**</span></span>
  
<span data-ttu-id="6acf0-107">קבל-תיבת דואר-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | הגדרת מ$true באמצעות תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="6acf0-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="6acf0-108">למד עוד</span><span class="sxs-lookup"><span data-stu-id="6acf0-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

