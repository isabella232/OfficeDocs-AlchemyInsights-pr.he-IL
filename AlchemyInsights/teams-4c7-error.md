---
title: שגיאה בצוותים 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796152"
---
# <a name="4c7-error-in-microsoft-teams"></a>שגיאת 4c7 בצוותי Microsoft

שגיאה זו מתרחשת מאחר שצוותי Microsoft דורשים אימות טפסים. בעת פריסת שירותי פדרציית הספריות של Active Directory (AD FS), אימות טפסים אינו מאופשר עבור האינטרא כברירת מחדל. אם האימות המשולב של Windows נכשל, תתבקש להיכנס באמצעות אימות טפסים.

כדי לפתור בעיה זו, הפוך את אימות הטפסים לזמין באמצעות יישום ה-snap-in של מסוף הניהול של Microsoft FS (MMC) במחשב המכיל את העותק המקומי של Active Directory. כדי לעשות זאת, בצע את הפעולות הבאות: 

1. בחלונית הניווט, דפדף אל **מדיניות אימות**.
2. תחת **פעולות** בחלונית הפרטים, בחר באפשרות **ערוך אימות ראשי כללי**.
3. בכרטיסיה **אינטרא-נט** , בחר באפשרות **אימות טפסים**.
4. בחר **ב'אישור '** (או **החל**).