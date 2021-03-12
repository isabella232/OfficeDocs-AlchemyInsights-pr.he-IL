---
title: שימוש ב-Exchange Online PowerShell כדי להפוך את DKIM לזמין עבור תחום ספציפי
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746280"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>שימוש ב-Exchange Online PowerShell כדי להפוך את DKIM לזמין עבור תחום ספציפי

אם אין באפשרותך ליצור את רשומות ה-DNS של DKIM במרכז הניהול, נסה להשתמש ב-Exchange Online PowerShell. 

כדי ליצור רשומת DNS של DKIM באמצעות Exchange Online PowerShell, בצע את השלבים הבאים:

1. פתח את Windows PowerShell כמנהל מערכת והפעלת הפקודות הבאות ברצף המתואר:

    מ. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
אם אתה נתקל בבעיות בהתחברות ל-Exchange Online PowerShell, ראה [התחברות אל Exchange Online powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. לאחר שאתה מחובר ל-Exchange Online PowerShell, הפעלת הפקודה הבאה:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. לאחר שהפקודה לעיל בוצעה בהצלחה, הפעל את הפקודה הבאה כדי לסיים את ההפעלה של Exchange Online PowerShell:

    `Remove-PSSession $Session` 



