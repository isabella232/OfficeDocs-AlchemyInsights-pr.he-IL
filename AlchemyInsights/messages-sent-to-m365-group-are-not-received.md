---
title: הודעות שנשלחות לקבוצת Microsoft 365 לא מתקבלות על-ידי כל החברים
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480684"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>הודעות שנשלחות לקבוצת Microsoft 365 לא מתקבלות על-ידי כל החברים

ודא שכל חברי הקבוצה נרשמו כמנויים לקבלת הודעות הדואר האלקטרוני. ראה [עקוב אחר קבוצה ב- Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

כדי לבדוק את מצב ההודעה של חברים שנרשמו כמנויים להודעות דואר אלקטרוני של קבוצה, הפעל את הפקודה הבאה ב- [PowerShell‏ EXO](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

השתמש בפקודה הבאה של EXO PowerShell כדי לקבוע שכל חברי הקבוצה יקבלו הודעות דואר אלקטרוני שנשלחות מקבוצת Microsoft 365 לתיבת הדואר הנכנס שלהם:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

לדוגמה:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`