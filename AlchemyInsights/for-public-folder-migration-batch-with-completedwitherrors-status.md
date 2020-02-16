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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043591"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="ad205-102">עבור אצוות העברה של תיקיות ציבוריות עם מצב מתחם שגיאות</span><span class="sxs-lookup"><span data-stu-id="ad205-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="ad205-103">השתמש בשלבים הבאים כדי להשלים את האצווה, בדילוג על הפריטים הגדולים/פגומים:</span><span class="sxs-lookup"><span data-stu-id="ad205-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="ad205-104">אשר את הפריטים שהמערכת דילגה עליהם באצוות העברה:</span><span class="sxs-lookup"><span data-stu-id="ad205-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="ad205-105">סט-MigrationBatch \<batchname>-מאשר הקיקיפמים</span><span class="sxs-lookup"><span data-stu-id="ad205-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="ad205-106">השתמש בפקודה הבאה כדי לאשר את הפריטים שהמערכת דילגה עליהם בבקשות העברה שאינן מסונכרנות אך לא הושלמו:</span><span class="sxs-lookup"><span data-stu-id="ad205-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="ad205-107">$pf = קבל-PublicFolderMailboxMigrationRequest | יציאה-PublicFolderMailboxMigrationRequestStatistics-כולל נמל; עבור כל ($i ב$pf) {אם ($i. ליגיפורט-gt 0-או $i. בדיחי-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. זהות. הקצאת מזהה ייחודי כללי-המשך $ ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="ad205-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="ad205-108">אצוות ההעברה והבקשות אמורות להמשיך ולהשלים בעוד מספר דקות.</span><span class="sxs-lookup"><span data-stu-id="ad205-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

