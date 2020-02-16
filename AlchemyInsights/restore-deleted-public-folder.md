---
title: שחזור תיקיה ציבורית שנמחקה
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063664"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="58b7c-102">שחזור תיקיה ציבורית שנמחקה</span><span class="sxs-lookup"><span data-stu-id="58b7c-102">Restore a deleted public folder</span></span>

<span data-ttu-id="58b7c-103">**כדי לשחזר פריטים שנמחקו מתיקיה ציבורית**:</span><span class="sxs-lookup"><span data-stu-id="58b7c-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="58b7c-104">ראה [אין באפשרותך לשחזר פריטים שנמחקו מתיקיה ציבורית שאינה דואר אלקטרוני ב-Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="58b7c-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="58b7c-105">**כדי לשחזר תיקיה ציבורית שנמחקה (מכל סוג שהוא)**:</span><span class="sxs-lookup"><span data-stu-id="58b7c-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="58b7c-106">אנא השתמש בעקבות הפקודה EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="58b7c-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="58b7c-107">תחביר</span><span class="sxs-lookup"><span data-stu-id="58b7c-107">Syntax:</span></span>

    ><span data-ttu-id="58b7c-108">$pf = קבל-ה התיקיה \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-רקורסיבי |? {$_. שם-eq "\<name_of_deleted_public_Folder"}; $Pf תיקיה מוגדרת-לפני הקובץ \<, נתיב הנתיב שבו התיקיה תהיה restored></span><span class="sxs-lookup"><span data-stu-id="58b7c-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="58b7c-109">דוגמה: הפקודה הבאה תשחזר את Subfolder1 ותמקם אותה תחת \הורות 1:</span><span class="sxs-lookup"><span data-stu-id="58b7c-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="58b7c-110">$pf = קבל-ה התיקיה \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-רקורסיבי |? {$_. שם-eq "Subfolder1"}; הגדרת תיקיה מוגדרת $pf. זהות-נתיב \ הורות 1</span><span class="sxs-lookup"><span data-stu-id="58b7c-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="58b7c-111">לקבלת פרטים נוספים, ראה [שחזור תיקיה ציבורית שנמחקה](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="58b7c-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
