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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995623"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams

ניתן לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams באמצעות [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/).  כל שעליך לעשות הוא לבחור את הקבוצה ולבחור @עריכת כתובת דואר אלקטרוני.

תוכל גם להשתמש בפקודת EXO PowerShell הבאה כדי לשנות את כתובת ה- SMTP הראשית של קבוצת Microsoft 365 / ‏Microsoft Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

דוגמה:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
