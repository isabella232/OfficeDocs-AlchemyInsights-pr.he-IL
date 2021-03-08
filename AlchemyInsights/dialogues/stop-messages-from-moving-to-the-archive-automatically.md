---
title: הפסקת העברת הודעות לארכיון באופן אוטומטי
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525103"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="e64d3-102">הפסקת העברת הודעות לארכיון באופן אוטומטי</span><span class="sxs-lookup"><span data-stu-id="e64d3-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="e64d3-103">אם אתה משתמש במדיניות שמירה, באפשרותך לשנות את גיל השמירה במדיניות זו כדי למנוע הודעות בארכיון באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="e64d3-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="e64d3-104">כך ניתן לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="e64d3-104">Here's how:</span></span>

1. <span data-ttu-id="e64d3-105">במרכז [הניהול של Exchange](https://go.microsoft.com/fwlink/?linkid=2059104), בחר   >  **תגיות שמירה** של ניהול תאימות.</span><span class="sxs-lookup"><span data-stu-id="e64d3-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="e64d3-106">אתר את המעבר אל תג שמירה בארכיון.</span><span class="sxs-lookup"><span data-stu-id="e64d3-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="e64d3-107">בתג השמירה, שנה את תקופת השמירה (תקופת הארכיון) כדי **לא** להפסיק את האחסון של פריטים בארכיון באופן אוטומטי על-ידי מדיניות שמירה.</span><span class="sxs-lookup"><span data-stu-id="e64d3-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="e64d3-108">פעולה זו תשנה את הגדרת הארכיון עבור כל תיבות הדואר שבהן הוחלה תגית שמירה זו.</span><span class="sxs-lookup"><span data-stu-id="e64d3-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
