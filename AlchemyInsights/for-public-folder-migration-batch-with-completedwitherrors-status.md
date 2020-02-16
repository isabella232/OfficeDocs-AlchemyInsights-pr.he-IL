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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>עבור אצוות העברה של תיקיות ציבוריות עם מצב מתחם שגיאות

השתמש בשלבים הבאים כדי להשלים את האצווה, בדילוג על הפריטים הגדולים/פגומים: 
1. אשר את הפריטים שהמערכת דילגה עליהם באצוות העברה:

    סט-MigrationBatch \<batchname>-מאשר הקיקיפמים 
2. השתמש בפקודה הבאה כדי לאשר את הפריטים שהמערכת דילגה עליהם בבקשות העברה שאינן מסונכרנות אך לא הושלמו:

    $pf = קבל-PublicFolderMailboxMigrationRequest | יציאה-PublicFolderMailboxMigrationRequestStatistics-כולל נמל; עבור כל ($i ב$pf) {אם ($i. ליגיפורט-gt 0-או $i. בדיחי-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. זהות. הקצאת מזהה ייחודי כללי-המשך $ ([DateTime]:: UtcNow)}}
3. אצוות ההעברה והבקשות אמורות להמשיך ולהשלים בעוד מספר דקות.

