---
title: התוספת teams עבור Mac
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670329"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="d7eda-102">התוספת teams עבור Mac</span><span class="sxs-lookup"><span data-stu-id="d7eda-102">Teams add-in for Mac</span></span>

<span data-ttu-id="d7eda-103">כדי לפתור בעיות של תוספת של צוותים חסרים עבור משתמשי מערכת ההפעלה של Mac, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="d7eda-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="d7eda-104">**שלב 1:** אם יש לך Exchange היברידי מקומי (2016 CU3 או מאוחר יותר נדרש), השתמש Test-HMA.ps1 בכלי כדי לאשר שאימות מודרני משולב מוגדר כהלכה.</span><span class="sxs-lookup"><span data-stu-id="d7eda-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="d7eda-105">לקבלת מידע נוסף, ראה [אימות הגדרת אימות מודרנית היברידית עבור Outlook עבור iOS ו-Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="d7eda-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="d7eda-106">**הערה** השתמש בתבנית כתובת UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)), לא domain\username.</span><span class="sxs-lookup"><span data-stu-id="d7eda-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="d7eda-107">עשה זאת גם עבור משתמשים בעלי תיבות דואר של Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d7eda-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="d7eda-108">**שלב 2:** העבר את המשתמש **Tools**  >  **לחשבונות**כלים... ב-Outlook עבור Mac, וחפש את החשבון ובחר אותו.</span><span class="sxs-lookup"><span data-stu-id="d7eda-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="d7eda-109">אשר את שם המשתמש המופיע בתבנית UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="d7eda-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="d7eda-110">**שלב 3:** אשר שהמשתמש הוא משתמש מורשה של Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d7eda-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="d7eda-111">על המשתמש להשתמש במנוי Office 365 for Mac, בגירסה 16.24 ואילך.</span><span class="sxs-lookup"><span data-stu-id="d7eda-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>