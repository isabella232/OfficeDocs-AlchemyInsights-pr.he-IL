---
title: חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746434"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="01900-102">חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך</span><span class="sxs-lookup"><span data-stu-id="01900-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="01900-103">בצע שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="01900-103">Follow these steps:</span></span>

1. <span data-ttu-id="01900-104">אם אינך מנהל מערכת כללי, כדי לחפש הודעות יש להוסיף את החשבון שלך **לקבוצת התפקידים ' מנהל גילוי אלקטרוני** ' או **לתפקיד ניהול חיפוש התאימות**.</span><span class="sxs-lookup"><span data-stu-id="01900-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="01900-105">כדי למחוק הודעות, יהיה עליך להצטרף **לקבוצת התפקידים ' ניהול ארגון** ' או **לתפקיד הניהול ' חיפוש וניקוי**'.</span><span class="sxs-lookup"><span data-stu-id="01900-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="01900-106">הרשאות לתפקידים אלה מוקצות [במרכז התאימות של אבטחה &.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="01900-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="01900-107">[צור חיפוש תוכן](https://docs.microsoft.com/office365/securitycompliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.</span><span class="sxs-lookup"><span data-stu-id="01900-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="01900-108">[התחבר אל מרכז התאימות של אבטחה & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="01900-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="01900-109">אם אתה משתמש במרכז המדינה, ראה הוראות אלה: [התחברות לאבטחה & מרכז התאימות של PowerShell באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="01900-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="01900-110">מחק את ההודעה: הפעיל את ה `New-ComplianceSearchAction` -cmdlet כדי למחוק את ההודעה.</span><span class="sxs-lookup"><span data-stu-id="01900-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="01900-111">הודעות שנמחקו מועברות לתיקיה ' פריטים הניתנים לשחזור ' של משתמש.</span><span class="sxs-lookup"><span data-stu-id="01900-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="01900-112">לקבלת פקודה לדוגמה, ראה [שלב 3: מחיקת ההודעה.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="01900-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
