---
title: אין אפשרות לגשת לתיקיות ציבוריות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891750"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="0b8ce-102">ל-Outlook אין אפשרות להתחבר לתיקיות ציבוריות</span><span class="sxs-lookup"><span data-stu-id="0b8ce-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="0b8ce-103">אם גישה לתיקיות ציבוריות אינה פועלת עבור משתמשים מסוימים, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0b8ce-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="0b8ce-104">התחבר ל-EXO PowerShell והגדר את הפרמטר DefaultPublicFolderMailbox Mailbox בחשבון המשתמש הבעייתי כדי להתאים לפרמטר בחשבון משתמש פעיל.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="0b8ce-105">דוגמה</span><span class="sxs-lookup"><span data-stu-id="0b8ce-105">Example:</span></span>

<span data-ttu-id="0b8ce-106">מקבל-תיבת דואר שלנו | תיבת דואר ברירת מלון ft, אפקטטfolder תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="0b8ce-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="0b8ce-107">מגדיר ברירת מcommand> של ברירת משתמש-ערך תיבת דואר \<של ברירת המשוב</span><span class="sxs-lookup"><span data-stu-id="0b8ce-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="0b8ce-108">המתן שעה אחת לפחות כדי שהשינוי ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="0b8ce-109">אם הבעיה נותרת, נא בצע [הליך זה](https://aka.ms/pfcte) כדי לפתור בעיות גישה לתיקיות ציבוריות באמצעות Outlook.</span><span class="sxs-lookup"><span data-stu-id="0b8ce-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>