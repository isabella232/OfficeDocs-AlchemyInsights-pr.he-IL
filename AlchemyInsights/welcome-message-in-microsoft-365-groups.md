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
# <a name="welcome-message-in-microsoft-365-groups"></a>הודעת ברוך הבא ב-Microsoft 365 קבוצות

משתמשים חדשים המצטרפים ל-Microsoft 365 לקבוצה יקבלו הודעת דואר מבורכת אם המאפיין "Uni, group Welהודעה זמינה" מתקיים.

במקרה שתרצה להשבית את הודעת הברכה, השתמש בפקודה [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) הבאה:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
