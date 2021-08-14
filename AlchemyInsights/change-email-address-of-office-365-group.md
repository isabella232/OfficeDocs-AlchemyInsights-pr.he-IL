---
title: שינוי כתובת דואר אלקטרוני של Microsoft 365 אישית
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
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930730"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>שינוי כתובת דואר אלקטרוני של Microsoft 365 אישית

באפשרותך לשנות את כתובת הדואר האלקטרוני של Microsoft 365 באמצעות מרכז הניהול. כל שעליך לעשות הוא לבחור את הקבוצה ולבחור @עריכת כתובת דואר אלקטרוני.

באפשרותך גם להשתמש בפקודה EXO PowerShell כדי לשנות את כתובת ה- SMTP הראשית של Microsoft 365 הבאה:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

דוגמה:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
