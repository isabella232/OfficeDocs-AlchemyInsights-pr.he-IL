---
title: הודעות שנשלחות לקבוצת Microsoft 365 לא מתקבלות על-ידי כל החברים
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976506"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>הודעות שנשלחות לקבוצת Microsoft 365 לא מתקבלות על-ידי כל החברים

ודא שכל חברי הקבוצה נרשמו כמנויים לקבלת הודעות הדואר האלקטרוני. ראה [עקוב אחר קבוצה ב- Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

כדי לבדוק את מצב ההודעה של חברים שנרשמו כמנויים להודעות דואר אלקטרוני של קבוצה, הפעל את הפקודה הבאה ב- [PowerShell‏ EXO](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

השתמש בפקודה הבאה של EXO PowerShell כדי לקבוע שכל חברי הקבוצה יקבלו הודעות דואר אלקטרוני שנשלחות מקבוצת Microsoft 365 לתיבת הדואר הנכנס שלהם:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

לדוגמה:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`