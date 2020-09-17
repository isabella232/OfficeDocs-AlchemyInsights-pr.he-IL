---
title: אין אפשרות לגשת לתיקיות ציבוריות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812548"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="57593-102">ל-Outlook אין אפשרות להתחבר לתיקיות ציבוריות</span><span class="sxs-lookup"><span data-stu-id="57593-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="57593-103">אם access public folder אינו עובד עבור חלק מהמשתמשים, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="57593-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="57593-104">התחבר ל-קליפת PowerShell וקבע את התצורה של הפרמטר DefaultPublicFolderMailbox בחשבון המשתמש של הבעיה כדי להתאים לפרמטר בחשבון משתמש עובד.</span><span class="sxs-lookup"><span data-stu-id="57593-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="57593-105">דוגמה</span><span class="sxs-lookup"><span data-stu-id="57593-105">Example:</span></span>

<span data-ttu-id="57593-106">קבלת-תיבת דואר WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="57593-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="57593-107">הגדרת תיבת דואר ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="57593-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="57593-108">המתן שעה אחת לפחות כדי שהשינוי ייכנס לתוקף.</span><span class="sxs-lookup"><span data-stu-id="57593-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="57593-109">אם הבעיה נשארת, בצע [הליך זה](https://aka.ms/pfcte) כדי לפתור בעיות בגישה לתיקיות ציבוריות באמצעות Outlook.</span><span class="sxs-lookup"><span data-stu-id="57593-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="57593-110">**כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook**:</span><span class="sxs-lookup"><span data-stu-id="57593-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="57593-111">שימוש ב-Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true או $false</span><span class="sxs-lookup"><span data-stu-id="57593-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="57593-112">$true: אפשר למשתמשים לגשת לתיקיות ציבוריות ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="57593-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="57593-113">$false: מנע גישת משתמשים לתיקיות ציבוריות ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="57593-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="57593-114">(אפס) זהו ערך ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="57593-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="57593-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="57593-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="57593-116">**הערה** הליך זה יכול לשלוט בחיבורים רק עם שולחן העבודה של Outlook עבור לקוחות Windows.</span><span class="sxs-lookup"><span data-stu-id="57593-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="57593-117">משתמש יכול להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="57593-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="57593-118">לקבלת מידע נוסף, ראה [הודעה על תמיכה בהתקשרויות מבוקרות לתיקיות ציבוריות ב-Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="57593-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>