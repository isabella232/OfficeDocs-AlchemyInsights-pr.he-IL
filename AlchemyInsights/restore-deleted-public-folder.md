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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158504"
---
# <a name="restore-a-deleted-public-folder"></a>שחזור תיקיה ציבורית שנמחקה

**כדי לשחזר פריטים שנמחקו מתיקיה ציבורית**:

- ראה [אין באפשרותך לשחזר פריטים שנמחקו מתיקיה ציבורית שאינה דואר אלקטרוני ב-Outlook 2016](https://aka.ms/pfrec).
 
**כדי לשחזר תיקיה ציבורית שנמחקה (מכל סוג שהוא)**: 

- אנא השתמש בעקבות הפקודה EXO PowerShell:

    תחביר

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    דוגמה: הפקודה הבאה תשחזר את Subfolder1 ותמקם אותה תחת \הורות 1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

לקבלת פרטים נוספים, ראה [שחזור תיקיה ציבורית שנמחקה](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
