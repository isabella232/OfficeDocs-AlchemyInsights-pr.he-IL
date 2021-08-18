---
title: AggregateGroupMailbox Full NDR שהתקבל עבור דואר אלקטרוני שנשלח Microsoft 365 הקבוצה
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315911"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox Full NDR שהתקבל עבור דואר אלקטרוני שנשלח Microsoft 365 הקבוצה

השתמש בפקודה הבאה של מעטפת EXO כדי ליצור כלל Exchange תעבורה כדי לשחרר באופן שקט הודעות דואר אלקטרוני שנשלחו לתיבת דואר של קבוצה מצטברת:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**הערה:** החלף את כתובת ה- SMTP **ב- -SentTo** בכתובת SMTP של תיבת הדואר של הקבוצה הצבירה הדייר שלך. באפשרותך לקבל את כתובת ה- SMTP של תיבת הדואר של הקבוצה הצבירה מה- NDR שהתקבל.



