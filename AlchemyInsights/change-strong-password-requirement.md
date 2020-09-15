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
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681873"
---
# <a name="change-strong-password-requirement"></a>שינוי דרישת סיסמה חזקה

Microsoft מחייבת סיסמאות חזקות כברירת מחדל. 

באמצעות PowerShell, באפשרותך להפוך סיסמאות חזקות ללא זמינות עבור משתמשים ספציפיים באמצעות פקודה זו:<br>
*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [מידע נוסף אודות מדיניות סיסמה](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [כיצד להתחבר ל-Microsoft 365 באמצעות PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [מידע נוסף אודות פקודות MsolUser של PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
