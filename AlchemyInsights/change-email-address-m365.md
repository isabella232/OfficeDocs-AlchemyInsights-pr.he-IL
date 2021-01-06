---
title: שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756558"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams

ניתן לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams באמצעות [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/).  כל שעליך לעשות הוא לבחור את הקבוצה ולבחור @עריכת כתובת דואר אלקטרוני.

תוכל גם להשתמש בפקודת EXO PowerShell הבאה כדי לשנות את כתובת ה- SMTP הראשית של קבוצת Microsoft 365 / ‏Microsoft Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

דוגמה:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
