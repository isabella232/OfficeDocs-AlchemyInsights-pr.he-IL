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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959496"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="20a73-102">ל-Outlook אין אפשרות להתחבר לתיקיות ציבוריות</span><span class="sxs-lookup"><span data-stu-id="20a73-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="20a73-103">אם הגישה לתיקיות ציבוריות אינה פועלת עבור משתמשים מעטים, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="20a73-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="20a73-104">התחבר ל-EXO PowerShell וקבע את התצורה של תיבת הדואר Defaultpublifolder בחשבון המשתמש הבעייתי כדי להתאים לאחד מחשבונות המשתמשים הפועלים.</span><span class="sxs-lookup"><span data-stu-id="20a73-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="20a73-105">דוגמה</span><span class="sxs-lookup"><span data-stu-id="20a73-105">Example:</span></span>

<span data-ttu-id="20a73-106">מקבל-תיבת דואר שלנו | תיבת דואר ברירת מלון ft, אפקטטfolder תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="20a73-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="20a73-107">מגדיר ברירת מcommand> של ברירת משתמש-ערך תיבת דואר \<של ברירת המשוב</span><span class="sxs-lookup"><span data-stu-id="20a73-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="20a73-108">המתן שעה אחת לפחות כדי שהשינוי ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="20a73-108">Wait at least one hour for the change to take effect.</span></span>