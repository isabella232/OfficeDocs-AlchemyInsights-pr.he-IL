---
title: הודעת ברוך הבא Microsoft 365 קבוצות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: 81127b79d4e5a16686ca46d67bfac73c15891938491a702219cd73757c4e106c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997711"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>הודעת ברוך הבא Microsoft 365 קבוצות

משתמשים חדשים שיצטרפו Microsoft 365 יקבלו דואר אלקטרוני בברכה אם המאפיין "UnifiedGroupWelcomeMessageEnabled" הוא True.

במקרה שברצונך להפוך את הודעת הפתיחה ללא זמינה, השתמש בפקודה [הבאה של EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
