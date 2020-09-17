---
title: שחזור תיקיה ציבורית שנמחקה
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774532"
---
# <a name="restore-a-deleted-public-folder"></a>שחזור תיקיה ציבורית שנמחקה

**כדי לשחזר פריטים שנמחקו מתיקיה ציבורית**:

- ראה [אין באפשרותך לשחזר פריטים שנמחקו מתיקיה ציבורית שאינה של mail ב-Outlook 2016](https://aka.ms/pfrec).
 
**כדי לשחזר תיקיה ציבורית שנמחקה (מכל סוג)**: 

- השתמש בפקודה הבאה ב-קליפת PowerShell:

    תחביר

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    דוגמה: הפקודה הבאה תשחזר את Subfolder1 ותמקם אותה תחת \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

ראה [שחזור תיקיה ציבורית שנמחקה](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) לקבלת פרטים נוספים.
