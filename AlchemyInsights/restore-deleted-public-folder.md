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
# <a name="restore-a-deleted-public-folder"></a>שחזור תיקיה ציבורית שנמחקה

**כדי לשחזר פריטים שנמחקו מתיקיה ציבורית**:

- ראה [אין באפשרותך לשחזר פריטים שנמחקו מתיקיה ציבורית שאינה דואר אלקטרוני ב-Outlook 2016](https://aka.ms/pfrec).
 
**כדי לשחזר תיקיה ציבורית שנמחקה (מכל סוג שהוא)**: 

- אנא השתמש בעקבות הפקודה EXO PowerShell:

    תחביר

    >$pf = קבל-ה התיקיה \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-רקורסיבי |? {$_. שם-eq "\<name_of_deleted_public_Folder"}; $Pf תיקיה מוגדרת-לפני הקובץ \<, נתיב הנתיב שבו התיקיה תהיה restored>

    דוגמה: הפקודה הבאה תשחזר את Subfolder1 ותמקם אותה תחת \הורות 1:

    >$pf = קבל-ה התיקיה \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-רקורסיבי |? {$_. שם-eq "Subfolder1"}; הגדרת תיקיה מוגדרת $pf. זהות-נתיב \ הורות 1

לקבלת פרטים נוספים, ראה [שחזור תיקיה ציבורית שנמחקה](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
