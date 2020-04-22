---
title: שינוי דרישת סיסמה חזקה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706562"
---
# <a name="change-strong-password-requirement"></a>שינוי דרישת סיסמה חזקה

מיקרוסופט דורשת סיסמאות חזקות כברירת מחדל. 

באמצעות PowerShell, אתה יכול להשבית סיסמאות חזקות עבור משתמשים ספציפיים עם פקודה זו:<br>
*סט-מוסולמשתמש-שם <UserPrincipalName> ה$false*

- [מידע נוסף על מדיניות הסיסמאות](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [כיצד להתחבר ל-Microsoft 365 עם PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [מידע נוסף על הפקודות של PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
