---
title: עבור אצוות העברה של תיקיות ציבוריות עם מצב מתחם שגיאות
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158608"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="c1c97-102">עבור אצוות העברה של תיקיות ציבוריות עם מצב מתחם שגיאות</span><span class="sxs-lookup"><span data-stu-id="c1c97-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="c1c97-103">השתמש בשלבים הבאים כדי להשלים את האצווה, בדילוג על הפריטים הגדולים/פגומים:</span><span class="sxs-lookup"><span data-stu-id="c1c97-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="c1c97-104">אשר את הפריטים שהמערכת דילגה עליהם באצוות העברה:</span><span class="sxs-lookup"><span data-stu-id="c1c97-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="c1c97-105">השתמש בפקודה הבאה כדי לאשר את הפריטים שהמערכת דילגה עליהם בבקשות העברה שאינן מסונכרנות אך לא הושלמו:</span><span class="sxs-lookup"><span data-stu-id="c1c97-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="c1c97-106">אצוות ההעברה והבקשות אמורות להמשיך ולהשלים בעוד מספר דקות.</span><span class="sxs-lookup"><span data-stu-id="c1c97-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

