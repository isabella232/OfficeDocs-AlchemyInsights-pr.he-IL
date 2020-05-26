---
title: הודעת ברוך הבא ב-Microsoft 365 קבוצות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357844"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="5483c-102">הודעת ברוך הבא ב-Microsoft 365 קבוצות</span><span class="sxs-lookup"><span data-stu-id="5483c-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="5483c-103">משתמשים חדשים המצטרפים ל-Microsoft 365 לקבוצה יקבלו הודעת דואר מבורכת אם המאפיין "Uni, group Welהודעה זמינה" מתקיים.</span><span class="sxs-lookup"><span data-stu-id="5483c-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="5483c-104">במקרה שתרצה להשבית את הודעת הברכה, השתמש בפקודה [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) הבאה:</span><span class="sxs-lookup"><span data-stu-id="5483c-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
