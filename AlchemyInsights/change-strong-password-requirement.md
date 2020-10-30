---
title: שינוי דרישת סיסמה חזקה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804424"
---
# <a name="change-strong-password-requirement"></a>שינוי דרישת סיסמה חזקה

Microsoft מחייבת סיסמאות חזקות כברירת מחדל.

באמצעות PowerShell, באפשרותך להפוך סיסמאות חזקות ללא זמינות עבור משתמשים ספציפיים באמצעות פקודות אלה:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

כדי להפוך סיסמאות חזקות ללא זמינות עבור כל המשתמשים, השתמש ב:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [מידע נוסף אודות מדיניות סיסמה](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [כיצד להתחבר ל-Microsoft 365 באמצעות PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [מידע נוסף אודות פקודות MsolUser של PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
