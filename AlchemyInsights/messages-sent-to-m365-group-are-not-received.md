---
title: הודעות הנשלחות לקבוצה של Microsoft 365 לא יתקבלו על-ידי כל החברים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: he-IL
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051498"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>הודעות הנשלחות לקבוצה של Microsoft 365 לא יתקבלו על-ידי כל החברים

ודא שכל חברי הקבוצה מנויים לקבלת הודעות דואר אלקטרוני. ראה [מעקב אחר קבוצה ב-Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

כדי לבדוק את מצב ההודעה של חברים שיש להם מנוי מיילים לקבוצה, הפעל את הפקודה הבאה ב- [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`