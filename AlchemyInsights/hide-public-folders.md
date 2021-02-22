---
title: הסתרת תיקיות ציבוריות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315371"
---
# <a name="hide-public-folders"></a><span data-ttu-id="df171-102">הסתרת תיקיות ציבוריות</span><span class="sxs-lookup"><span data-stu-id="df171-102">Hide public folders</span></span>

<span data-ttu-id="df171-103">**כדי להסתיר את עץ התיקיות הציבוריות כולו**:</span><span class="sxs-lookup"><span data-stu-id="df171-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="df171-104">השתמש בשלבים המפורטים במאמר [זה](https://aka.ms/ControlPF) כדי להסתיר את כל עץ התיקיות הציבוריות מתוך בררני או כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="df171-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="df171-105">**כדי להסתיר תיקיה ציבורית ספציפית**:</span><span class="sxs-lookup"><span data-stu-id="df171-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="df171-106">הוספת הרשאות עבור משתמשים שצריכים לגשת לתיקיה הציבורית</span><span class="sxs-lookup"><span data-stu-id="df171-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="df171-107">הסר את **ברירת המחדל** של המשתמש מרשימת **ההרשאות** :</span><span class="sxs-lookup"><span data-stu-id="df171-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
