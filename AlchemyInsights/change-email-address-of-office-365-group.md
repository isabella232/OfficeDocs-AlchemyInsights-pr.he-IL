---
title: שינוי כתובת הדואר האלקטרוני של קבוצת מיקרוסופט 365
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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580658"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>שינוי כתובת הדואר האלקטרוני של קבוצת מיקרוסופט 365

באפשרותך לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 באמצעות מרכז הניהול. פשוט בחר את הקבוצה ובחר את כתובת הדוא @edit.

באפשרותך גם להשתמש בעקבות הפקודה EXO PowerShell כדי לשנות את כתובת ה-SMTP הראשית של קבוצת Microsoft 365:

קבוצת מערכת-יוניסט <Group Name> -PrimarySmtpAddress<new SMTP Address>

דוגמה

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
