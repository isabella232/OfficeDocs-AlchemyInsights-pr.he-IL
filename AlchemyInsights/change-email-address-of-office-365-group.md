---
title: שינוי כתובת דואר אלקטרוני של קבוצה של Microsoft 365
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819045"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>שינוי כתובת דואר אלקטרוני של קבוצה של Microsoft 365

באפשרותך לשנות את כתובת הדואר האלקטרוני של קבוצה של Microsoft 365 באמצעות מרכז הניהול. כל שעליך לעשות הוא לבחור את הקבוצה ולבחור @עריכת כתובת דואר אלקטרוני.

באפשרותך גם להשתמש בפקודה EXO PowerShell כדי לשנות את כתובת ה- SMTP הראשית של קבוצה של Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

דוגמה:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
