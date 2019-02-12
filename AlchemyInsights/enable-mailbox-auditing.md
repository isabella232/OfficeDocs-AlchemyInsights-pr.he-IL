---
title: אפשר ביקורת של תיבת דואר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 3a7ffccadf6b415f7dd0d0871d368402332a0cd7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916741"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="80b3a-102">אפשר ביקורת של תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="80b3a-102">Enable mailbox auditing</span></span>

<span data-ttu-id="80b3a-103">כדי להפעיל ביקורת על-ידי תיבת הדואר עבור משתמש בודד או ארגון שלם יש להפעיל את כלי cmdlet הבאים ממעטפת ההפעלה מרחוק:</span><span class="sxs-lookup"><span data-stu-id="80b3a-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="80b3a-104">**משתמש יחיד**</span><span class="sxs-lookup"><span data-stu-id="80b3a-104">**Single User**</span></span>
  
<span data-ttu-id="80b3a-105">Set-Mailbox - זהות "יורם חלון" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="80b3a-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="80b3a-106">**הארגון**</span><span class="sxs-lookup"><span data-stu-id="80b3a-106">**Organization**</span></span>
  
<span data-ttu-id="80b3a-107">תיבת דואר-get - ResultSize מוגבל - סינון {"UserMailbox" RecipientTypeDetails - eq} | Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="80b3a-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="80b3a-108">מידע נוסף</span><span class="sxs-lookup"><span data-stu-id="80b3a-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

