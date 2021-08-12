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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943376"
---
# <a name="restore-a-deleted-public-folder"></a>שחזור תיקיה ציבורית שנמחקה

**כדי לשחזר פריטים שנמחקו מתיקיה ציבורית**:

- ראה [אין באפשרותך לשחזר פריטים שנמחקו מתיקיה ציבורית](https://aka.ms/pfrec)שאינו דואר אלקטרוני ב- Outlook 2016 .
 
**כדי לשחזר תיקיה ציבורית שנמחקה (מכל סוג)**: 

- השתמש בפקודה הבאה של EXO PowerShell:

    תחביר:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    דוגמה: הפקודה הבאה תשחזר את תיקיית המשנה1 ות למקם אותה תחת \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

ראה [שחזור תיקיה ציבורית שנמחקה](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) לקבלת פרטים נוספים.
