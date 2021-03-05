---
title: 'כדי לקבוע מענה אוטומטי עבור כל הודעות הדואר האלקטרוני הנשלחות לקבוצה של Microsoft 365:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481859"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>כדי לקבוע מענה אוטומטי עבור כל הודעות הדואר האלקטרוני הנשלחות לקבוצה של Microsoft 365:

**התחבר ל-קליפת PowerShell באמצעות חשבון מנהל הדיירים והשתמש בפקודה הבאה**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> שנה את **groupmailbox** לשם קבוצה שבו ברצונך לקבוע את התצורה של מענה אוטומטי.

