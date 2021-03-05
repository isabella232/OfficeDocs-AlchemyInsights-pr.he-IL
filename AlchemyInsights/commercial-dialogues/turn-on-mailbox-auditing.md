---
title: הפעלת ביקורת תיבת דואר
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482467"
---
# <a name="turn-on-mailbox-auditing"></a>הפעלת ביקורת תיבת דואר

כדי להפעיל את ביקורת תיבת הדואר עבור משתמש בודד או ארגון שלם, הפעל את רכיבי ה-cmdlet הבאים מ-PowerShell מרוחק:

- **משתמש בודד**: Set-Mailbox-זהות "AuditEnabled דאו"-$true
- **ארגון**: Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-Eq "UserMailbox"} | Set-Mailbox-AuditEnabled $true

לקבלת מידע נוסף, ראה [ניהול ביקורת של תיבות דואר](https://go.microsoft.com/fwlink/?linkid=2103668).