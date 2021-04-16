---
title: שחזור תיקיה ציבורית שנמחקה
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809440"
---
# <a name="restore-a-deleted-public-folder"></a>שחזור תיקיה ציבורית שנמחקה

**כדי לשחזר פריטים שנמחקו מתיקיה ציבורית**:

- ראה אין באפשרותך לשחזר פריטים שנמחקו מתיקיה ציבורית שאינו דואר [אלקטרוני ב- Outlook 2016](https://aka.ms/pfrec).
 
**כדי לשחזר תיקיה ציבורית שנמחקה (מכל סוג)**: 

- השתמש בפקודה הבאה של EXO PowerShell:

    תחביר:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    דוגמה: הפקודה הבאה תשחזר את תיקיית המשנה1 ות למקם אותה תחת \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

ראה [שחזור תיקיה ציבורית שנמחקה](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) לקבלת פרטים נוספים.
