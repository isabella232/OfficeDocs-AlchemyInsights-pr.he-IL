---
title: עבור אצוות העברה של תיקיות ציבוריות באמצעות מצב CompletedWithErrors
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744114"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>עבור אצוות העברה של תיקיות ציבוריות באמצעות מצב CompletedWithErrors

השתמש בשלבים הבאים כדי להשלים את האצווה, ולדלג על הפריטים הגדולים/הרעים: 
1. אשר את הפריטים שדילגת עליהם באצוות ההעברה:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. השתמש בפקודה הבאה כדי לאשר את הפריטים שהמערכת דילגה עליהם בבקשות העברה שסונכרנו "אך לא הושלמו:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. אצוות ההעברה ובקשות אמורות לחדש ולהשלים תוך כמה דקות.

