---
title: שליטה בגישה לתיקיות ציבוריות באמצעות Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816741"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="33a66-102">שליטה בגישה לתיקיות ציבוריות באמצעות Outlook</span><span class="sxs-lookup"><span data-stu-id="33a66-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="33a66-103">כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook:</span><span class="sxs-lookup"><span data-stu-id="33a66-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="33a66-104">השתמש ב- `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="33a66-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="33a66-105">$true: אפשר למשתמשים לגשת לתיקיות ציבוריות ב- Outlook</span><span class="sxs-lookup"><span data-stu-id="33a66-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="33a66-106">$false: מניעת גישת משתמש לתיקיות ציבוריות ב- Outlook.</span><span class="sxs-lookup"><span data-stu-id="33a66-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="33a66-107">(אפס) זהו ערך ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="33a66-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="33a66-108">הערה: הליך זה יכול לשלוט רק בחיבורים עם שולחן העבודה של Outlook עבור לקוחות Windows.</span><span class="sxs-lookup"><span data-stu-id="33a66-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="33a66-109">המשתמשים יכולים להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook עבור Mac.</span><span class="sxs-lookup"><span data-stu-id="33a66-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="33a66-110">לקבלת מידע נוסף, ראה [חיבורים מבוקרים לתיקיות ציבוריות ב- Outlook](https://aka.ms/controlpf) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="33a66-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
