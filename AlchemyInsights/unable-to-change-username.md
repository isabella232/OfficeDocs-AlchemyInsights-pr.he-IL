---
title: אין אפשרות לשנות שם משתמש
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439551"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="0dfec-102">אין אפשרות לשנות שם משתמש</span><span class="sxs-lookup"><span data-stu-id="0dfec-102">Unable to change UserName</span></span>

<span data-ttu-id="0dfec-103">במקרים מסוימים, השינויים ב-UPN (שם המשתמש) אינם מופצים לענן הצמתים.</span><span class="sxs-lookup"><span data-stu-id="0dfec-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="0dfec-104">ייתכן שתקבל שגיאות אימות בפורטל של Office 365 או שלא תוכל לשנות את שם המשתמש או את כתובת הדואר האלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="0dfec-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="0dfec-105">כדי לפתור בעיה זו, הגדר באופן ידני את שם המשתמש באמצעות פקודה PowerShell זו.</span><span class="sxs-lookup"><span data-stu-id="0dfec-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="0dfec-106">**דוגמה: שינוי שם של משתמש**</span><span class="sxs-lookup"><span data-stu-id="0dfec-106">**Example: Rename a user**</span></span>

<span data-ttu-id="0dfec-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="0dfec-107">PowerShellCopy</span></span>

<span data-ttu-id="0dfec-108">נ. ב.: \> Set-Msoluserהפריפלשם-מdavidc@contoso.com שם המשתמש "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="0dfec-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="0dfec-109">פקודה זו שינוי שם הdavidc@contoso.com לdavidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="0dfec-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="0dfec-110">לקבלת מידע נוסף, ראה [הגדרת משתמשים בשמות](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="0dfec-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>