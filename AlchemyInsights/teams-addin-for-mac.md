---
title: Teams תוספת עבור Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582071"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="1877f-102">Teams תוספת עבור Mac</span><span class="sxs-lookup"><span data-stu-id="1877f-102">Teams add-in for Mac</span></span>

<span data-ttu-id="1877f-103">כדי לפתור בעיות של Teams עבור משתמשי מערכת ההפעלה Mac, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1877f-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="1877f-104">**שלב 1:** אם יש לך Exchange היברידי מקומי (2016 CU3 ואילך נדרש), השתמש בכלי Test-HMA.ps1 כדי לוודא שתצורת האימות המודרנית ההיברידית נקבעה כראוי.</span><span class="sxs-lookup"><span data-stu-id="1877f-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="1877f-105">לקבלת מידע נוסף, ראה [אימות הגדרת אימות מודרני היברידי עבור Outlook עבור iOS ו- Android](https://aka.ms/TestHMAEAS).</span><span class="sxs-lookup"><span data-stu-id="1877f-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="1877f-106">**הערה** השתמש בתבנית כתובת UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)), ולא domain\username.</span><span class="sxs-lookup"><span data-stu-id="1877f-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="1877f-107">בצע פעולה זו גם עבור משתמשים בעלי Exchange Online דואר.</span><span class="sxs-lookup"><span data-stu-id="1877f-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="1877f-108">**שלב 2:** האם המשתמש י לעבור אל **'חשבונות**  >  **כלים'**... ב- Outlook עבור Mac, ומצא ובחר את החשבון.</span><span class="sxs-lookup"><span data-stu-id="1877f-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="1877f-109">אשר את שם המשתמש המפורט בתבנית UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="1877f-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="1877f-110">**שלב 3:** אשר שהמשתמש הוא משתמש מורשה Microsoft Teams משתמש.</span><span class="sxs-lookup"><span data-stu-id="1877f-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="1877f-111">המשתמש חייב להשתמש במנוי Office 365 עבור Mac, במוצר גירסה 16.24 ואילך.</span><span class="sxs-lookup"><span data-stu-id="1877f-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>