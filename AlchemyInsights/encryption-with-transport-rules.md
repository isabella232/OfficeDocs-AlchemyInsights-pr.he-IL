---
title: הצפנה באמצעות כללי תעבורה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915178"
---
# <a name="encryption-with-transport-rules"></a>הצפנה באמצעות כללי תעבורה

ב[מרכז הניהול של Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), באפשרותך להשתמש ביכולות של הצפנת הודעות של Office (OME) בכללי זרימת הדואר כדי להפעיל הצפנת הודעות. בחר את האפשרות **החל הצפנת הודעות והגנת זכויות של Office 365** בתנאי כלל התעבורה.

- לקבלת מידע נוסף, ראה [הגדר את כלל זרימת הדואר כדי להצפין](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- ב- Powershell, השתמש ברכיב ה- cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) והגדר את הפרמטר *ApplyOME* ל- $true.
