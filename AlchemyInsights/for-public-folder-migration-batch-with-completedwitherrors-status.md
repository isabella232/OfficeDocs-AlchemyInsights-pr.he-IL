---
title: עבור אצוות העברה של תיקיה ציבורית עם מצב CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812465"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>עבור אצוות העברה של תיקיה ציבורית עם מצב CompletedWithErrors

בצע את השלבים הבאים כדי להשלים את האצווה, דילוג על הפריטים הגדולים/הרעים: 
1. אשר את הפריטים המדלגים על אצוות העברה:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. השתמש בפקודה הבאה כדי לאשר את הפריטים המדלגים על בקשות העברה ש"מסונכרנים" אך לא הושלמו:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. אצוות ההעברה והבקשות אמורות לחדש ולהשלים בתוך כמה דקות.

