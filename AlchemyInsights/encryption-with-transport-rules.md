---
title: הצפנה באמצעות כללי תעבורה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079451"
---
# <a name="encryption-with-transport-rules"></a>הצפנה באמצעות כללי תעבורה

ב[מרכז הניהול של Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), באפשרותך להשתמש ביכולות של הצפנת הודעות של Office (OME) בכללי זרימת הדואר כדי להפעיל הצפנת הודעות. בחר את האפשרות **החל הצפנת הודעות והגנת זכויות של Office 365** בתנאי כלל התעבורה.

- לקבלת מידע נוסף, ראה [הגדר את כלל זרימת הדואר כדי להצפין](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- ב- Powershell, השתמש ברכיב ה- cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) והגדר את הפרמטר *ApplyOME* ל- $true.
