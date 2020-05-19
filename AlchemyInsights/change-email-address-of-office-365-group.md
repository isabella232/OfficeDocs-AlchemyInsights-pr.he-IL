---
title: שינוי כתובת הדואר האלקטרוני של קבוצת Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282923"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>שינוי כתובת הדואר האלקטרוני של קבוצת Microsoft 365

באפשרותך לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 באמצעות מרכז הניהול. פשוט בחר את הקבוצה ובחר את כתובת הדוא @edit.

באפשרותך גם להשתמש בעקבות הפקודה EXO PowerShell כדי לשנות את כתובת ה-SMTP הראשית של קבוצת Microsoft 365:

קבוצת מערכת-יוניסט <Group Name> -PrimarySmtpAddress<new SMTP Address>

דוגמה

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
