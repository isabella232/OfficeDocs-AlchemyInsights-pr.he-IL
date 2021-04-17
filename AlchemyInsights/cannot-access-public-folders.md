---
title: אין אפשרות לגשת לתיקיות ציבוריות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819513"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="c6d41-102">ל- Outlook אין אפשרות להתחבר לתיקיות ציבוריות</span><span class="sxs-lookup"><span data-stu-id="c6d41-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="c6d41-103">אם הגישה לתיקיה ציבורית אינה פועלת עבור משתמשים מסוימים, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c6d41-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="c6d41-104">התחבר ל- EXO PowerShell והגדר את הפרמטר DefaultPublicFolderMailbox בחשבון המשתמש הלבעיה כך שיתאים לפרמטר בחשבון משתמש פועל.</span><span class="sxs-lookup"><span data-stu-id="c6d41-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="c6d41-105">דוגמה:</span><span class="sxs-lookup"><span data-stu-id="c6d41-105">Example:</span></span>

<span data-ttu-id="c6d41-106">Get-Mailbox WorkingUser | ft DefaultציבוריFolderMailbox,EffectiveציבוריFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="c6d41-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="c6d41-107">Set-Mailbox בעיהUser -DefaultציבוריFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="c6d41-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="c6d41-108">המתן לפחות שעה אחת עד שהשינוי יתוקף.</span><span class="sxs-lookup"><span data-stu-id="c6d41-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="c6d41-109">אם הבעיה נשארת, בצע הליך זה [כדי לפתור](https://aka.ms/pfcte) בעיות גישה לתיקיה ציבורית באמצעות Outlook.</span><span class="sxs-lookup"><span data-stu-id="c6d41-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="c6d41-110">**כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook**:</span><span class="sxs-lookup"><span data-stu-id="c6d41-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="c6d41-111">השתמש <mailboxname> Set-CASMailbox-PublicFolderClientAccess $true או $false</span><span class="sxs-lookup"><span data-stu-id="c6d41-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="c6d41-112">$true: אפשר למשתמשים לגשת לתיקיות ציבוריות ב- Outlook</span><span class="sxs-lookup"><span data-stu-id="c6d41-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="c6d41-113">$false: מניעת גישת משתמש לתיקיות ציבוריות ב- Outlook.</span><span class="sxs-lookup"><span data-stu-id="c6d41-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="c6d41-114">(אפס) זהו ערך ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="c6d41-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="c6d41-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="c6d41-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="c6d41-116">**הערה** הליך זה יכול לשלוט בחיבורים רק עם שולחן העבודה של Outlook עבור לקוחות Windows.</span><span class="sxs-lookup"><span data-stu-id="c6d41-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="c6d41-117">משתמש יכול להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook עבור Mac.</span><span class="sxs-lookup"><span data-stu-id="c6d41-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="c6d41-118">לקבלת מידע נוסף, ראה [הודעה על תמיכה עבור חיבורים מבוקרים לתיקיות ציבוריות ב- Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="c6d41-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>