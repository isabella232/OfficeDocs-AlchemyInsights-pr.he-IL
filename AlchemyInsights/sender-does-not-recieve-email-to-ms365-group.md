---
title: השולח אינו מקבל דואר אלקטרוני שנשלח לקבוצה של Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871848"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>השולח אינו מקבל דואר אלקטרוני שנשלח לקבוצה של Microsoft 365

כברירת מחדל, השולח של הודעת דואר אלקטרוני לקבוצה של Microsoft 365 אינו מקבל עותק של ההודעה בתיבת הדואר הנכנס שלהם, גם אם השולח הוא חבר בקבוצה.

השתמש בפקודה זו של קליפת PowerShell כדי לאפשר לשולח לקבל עותק של כל דואר אלקטרוני שהם שולחים לקבוצה של Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

כדי להפוך את ההגדרה עבור כל תיבות הדואר בו:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**הערה** שינויים בהגדרה זו נמשכים שעה כדי להיכנס לתוקף.