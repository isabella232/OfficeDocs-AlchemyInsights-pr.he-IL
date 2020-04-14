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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286264"
---
# <a name="change-strong-password-requirement"></a>שינוי דרישת סיסמה חזקה

מיקרוסופט דורשת סיסמאות חזקות כברירת מחדל. 

באמצעות PowerShell, אתה יכול להשבית סיסמאות חזקות עבור משתמשים ספציפיים עם פקודה זו:<br>
*סט-מוסולמשתמש-שם <UserPrincipalName> ה$false*

- [מידע נוסף על מדיניות הסיסמאות](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [כיצד להתחבר ל-Office 365 עם PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [מידע נוסף על הפקודות של PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [הגדרת סיסמאות משתמש עם תוקף שלא יפוג לעולם](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
