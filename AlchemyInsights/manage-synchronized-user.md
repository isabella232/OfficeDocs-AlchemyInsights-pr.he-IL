---
title: ניהול המשתמש מסונכרן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541996"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="5ead0-102">אין אפשרות להגדיר כתובת דואר אלקטרוני ראשית או לשנות תכונות משתמש</span><span class="sxs-lookup"><span data-stu-id="5ead0-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="5ead0-103">אם סינכרון ספריות זמין עבור הסביבה שלך, אין אפשרות לשנות תכונות מסוימות למשתמש או לאובייקט Microsoft 365 admin למרכז.</span><span class="sxs-lookup"><span data-stu-id="5ead0-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="5ead0-104">כדי לנהל באופן מלא כל התכונות שלהם ומשתמשים מסונכרן, השתמש שלך אקטיבית מקומיים משתמשים וקבוצות במסוף ניהול (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="5ead0-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="5ead0-105">לחלופין, באפשרותך לשנות משתמשים בודדים או תכונות עבור משתמשים מסונכרנים באמצעות powershell כגון שמוצג בדוגמאות אלה נפוצים:</span><span class="sxs-lookup"><span data-stu-id="5ead0-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="5ead0-106">ערכת-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5ead0-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="5ead0-107">ערכת-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "משתמש בדיקה" - שם משפחה "משתמש"-כותרת "Manager"-מחלקה "משאבי אנוש"</span><span class="sxs-lookup"><span data-stu-id="5ead0-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="5ead0-108">הסר-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5ead0-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>