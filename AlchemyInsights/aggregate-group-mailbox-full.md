---
title: AggregateGroupMailbox מלא של NDR שהתקבל עבור דואר אלקטרוני שנשלח לקבוצה של Microsoft 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721919"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox מלא של NDR שהתקבל עבור דואר אלקטרוני שנשלח לקבוצה של Microsoft 365

השתמש בפקודה הבאה קליפת Shell כדי ליצור כלל תעבורה של Exchange כדי לשחרר הודעות דואר אלקטרוני שנשלחות לתיבת הדואר של קבוצת צבירה:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> החלף את כתובת ה-SMTP ב **-SentTo** עם כתובת smtp של תיבת הדואר של קבוצת צבירה בדייר שלך. באפשרותך לקבל את כתובת ה-SMTP של תיבת הדואר של קבוצת צבירה מ-NDR שהתקבל.



