---
title: שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819081"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams

ניתן לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams באמצעות [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/).  כל שעליך לעשות הוא לבחור את הקבוצה ולבחור @עריכת כתובת דואר אלקטרוני.

תוכל גם להשתמש בפקודת EXO PowerShell הבאה כדי לשנות את כתובת ה- SMTP הראשית של קבוצת Microsoft 365 / ‏Microsoft Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

דוגמה:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
