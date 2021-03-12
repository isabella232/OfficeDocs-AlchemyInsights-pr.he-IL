---
title: מדיניות סיסמאות
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744986"
---
# <a name="password-policies"></a><span data-ttu-id="47a64-102">מדיניות סיסמאות</span><span class="sxs-lookup"><span data-stu-id="47a64-102">Password policies</span></span>

<span data-ttu-id="47a64-103">**אני נתקל בבעיות במדיניות הסיסמה עבור משתמש**</span><span class="sxs-lookup"><span data-stu-id="47a64-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="47a64-104">מדיניות הסיסמה עבור משתמש תלויה בשאלה אם המשתמש הוא ענן בלבד או מקומי.</span><span class="sxs-lookup"><span data-stu-id="47a64-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="47a64-105">משתמשים בענן בלבד חייבים לבחור סיסמה העונה על הדרישות במאמר זה: [פריטי מדיניות סיסמה החלים רק על חשבונות משתמשים בענן](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="47a64-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="47a64-106">משתמשים מקומיים חייבים לבחור סיסמה העונה על הדרישות המקומיות.</span><span class="sxs-lookup"><span data-stu-id="47a64-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="47a64-107">אם למשתמש מקומי אין אפשרות להגדיר את הסיסמה שלו, בדוק את הדרישות המקומיות.</span><span class="sxs-lookup"><span data-stu-id="47a64-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="47a64-108">**איני יודע כיצד להגדיר או לבדוק מדיניות תפוגת סיסמאות**</span><span class="sxs-lookup"><span data-stu-id="47a64-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="47a64-109">באפשרותך להגדיר ולבדוק את מדיניות התפוגה של משתמשי הענן בדייר שלך באמצעות PowerShell.</span><span class="sxs-lookup"><span data-stu-id="47a64-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="47a64-110">בצע את ההוראות במאמר זה: [הגדר או בדוק את מדיניות הסיסמה באמצעות PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="47a64-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="47a64-111">מדיניות תפוגת הסיסמאות עבור משתמשים מקומיים מוגדרת במודעה המקומית שלך.</span><span class="sxs-lookup"><span data-stu-id="47a64-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="47a64-112">**קישורים שימושיים נוספים:**</span><span class="sxs-lookup"><span data-stu-id="47a64-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="47a64-113">תחילת העבודה עם איפוס סיסמה</span><span class="sxs-lookup"><span data-stu-id="47a64-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="47a64-114">פתרון בעיות באיפוס סיסמה המופעל על-ידי מנהל</span><span class="sxs-lookup"><span data-stu-id="47a64-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
