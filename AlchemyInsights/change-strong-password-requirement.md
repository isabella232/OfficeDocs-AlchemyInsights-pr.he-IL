---
title: דרישת סיסמה חזקה של שינוי
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
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518760"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="169ae-102">דרישת סיסמה חזקה של שינוי</span><span class="sxs-lookup"><span data-stu-id="169ae-102">Change strong password requirement</span></span>

<span data-ttu-id="169ae-103">כברירת מחדל, מיקרוסופט דורשת סיסמאות חזקות.</span><span class="sxs-lookup"><span data-stu-id="169ae-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="169ae-104">באמצעות PowerShell, באפשרותך להשבית סיסמאות חזקות עבור משתמשים מסוימים באמצעות פקודה זו:</span><span class="sxs-lookup"><span data-stu-id="169ae-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="169ae-105">*ערכת-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="169ae-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="169ae-106">מידע נוסף על מדיניות סיסמה</span><span class="sxs-lookup"><span data-stu-id="169ae-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="169ae-107">כיצד להתחבר Office 365 עם PowerShell</span><span class="sxs-lookup"><span data-stu-id="169ae-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="169ae-108">מידע נוסף אודות פקודות PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="169ae-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)