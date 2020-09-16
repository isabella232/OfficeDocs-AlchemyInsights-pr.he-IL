---
title: הפיכת ביקורת תיבת דואר לזמינה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806292"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="6e483-102">הפיכת ביקורת תיבת דואר לזמינה</span><span class="sxs-lookup"><span data-stu-id="6e483-102">Enable mailbox auditing</span></span>

<span data-ttu-id="6e483-103">כדי להפוך ביקורת של תיבות דואר לזמינה עבור משתמש בודד או של ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים מתוך מעטפת Power מרוחקת:</span><span class="sxs-lookup"><span data-stu-id="6e483-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="6e483-104">**משתמש בודד**</span><span class="sxs-lookup"><span data-stu-id="6e483-104">**Single User**</span></span>
  
<span data-ttu-id="6e483-105">Set-תיבת דואר-זהות "ג'יין דאו"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="6e483-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="6e483-106">**ארגון**</span><span class="sxs-lookup"><span data-stu-id="6e483-106">**Organization**</span></span>
  
<span data-ttu-id="6e483-107">Get-Mailbox-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | Set-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="6e483-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="6e483-108">למד עוד</span><span class="sxs-lookup"><span data-stu-id="6e483-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

