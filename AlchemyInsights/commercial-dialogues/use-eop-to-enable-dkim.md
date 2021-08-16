---
title: השתמש Exchange Online PowerShell כדי להפוך את DKIM לזמין עבור תחום ספציפי
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070302"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>השתמש Exchange Online PowerShell כדי להפוך את DKIM לזמין עבור תחום ספציפי

אם אינך יכול ליצור את רשומות ה- DNS של DKIM במרכז הניהול, נסה להשתמש ב- Exchange Online PowerShell. 

כדי ליצור רשומת DNS של DKIM באמצעות Exchange Online PowerShell, בצע את השלבים הבאים:

1. פתח Windows PowerShell כמנהל מערכת ולהפעיל את הפקודות הבאות ברצף המתואר:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
אם אתה מתקשה להתחבר Exchange Online PowerShell, [ראה התחברות כדי Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. לאחר שאתה מחובר ל- Exchange Online PowerShell, הפעל את הפקודה הבאה:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. לאחר ביצוע הפקודה לעיל בהצלחה, הפעל את הפקודה הבאה כדי לסיים את הפעלת Exchange Online PowerShell:

    `Remove-PSSession $Session` 



