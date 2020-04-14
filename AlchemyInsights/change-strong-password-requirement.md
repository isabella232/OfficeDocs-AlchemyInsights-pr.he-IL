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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="10178-102">שינוי דרישת סיסמה חזקה</span><span class="sxs-lookup"><span data-stu-id="10178-102">Change strong password requirement</span></span>

<span data-ttu-id="10178-103">מיקרוסופט דורשת סיסמאות חזקות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="10178-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="10178-104">באמצעות PowerShell, אתה יכול להשבית סיסמאות חזקות עבור משתמשים ספציפיים עם פקודה זו:</span><span class="sxs-lookup"><span data-stu-id="10178-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="10178-105">*סט-מוסולמשתמש-שם <UserPrincipalName> ה$false*</span><span class="sxs-lookup"><span data-stu-id="10178-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="10178-106">מידע נוסף על מדיניות הסיסמאות</span><span class="sxs-lookup"><span data-stu-id="10178-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="10178-107">כיצד להתחבר ל-Office 365 עם PowerShell</span><span class="sxs-lookup"><span data-stu-id="10178-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="10178-108">מידע נוסף על הפקודות של PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="10178-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="10178-109">הגדרת סיסמאות משתמש עם תוקף שלא יפוג לעולם</span><span class="sxs-lookup"><span data-stu-id="10178-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
