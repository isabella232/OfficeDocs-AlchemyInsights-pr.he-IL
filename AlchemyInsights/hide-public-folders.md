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
# <a name="hide-public-folders"></a>הסתרת תיקיות ציבוריות

**כדי להסתיר את עץ התיקיות הציבוריות כולו**:

השתמש בשלבים המפורטים במאמר [זה](https://aka.ms/ControlPF) כדי להסתיר את כל עץ התיקיות הציבוריות מתוך בררני או כל המשתמשים.

**כדי להסתיר תיקיה ציבורית ספציפית**:

1. הוספת הרשאות עבור משתמשים שצריכים לגשת לתיקיה הציבורית

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. הסר את **ברירת המחדל** של המשתמש מרשימת **ההרשאות** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
