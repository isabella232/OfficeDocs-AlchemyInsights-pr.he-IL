---
title: שגיאת teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700204"
---
# <a name="4c7-error-in-microsoft-teams"></a>שגיאה של 4c7 ב-Microsoft Teams

שגיאה זו מתרחשת מאחר ש-Microsoft Teams דורש אימות טפסים. בעת פריסת שירותי האיחוד של Active Directory (AD FS), אימות טפסים אינו זמין עבור האינטרא כברירת מחדל. אם האימות המשולב של Windows נכשל, אתה מתבקש להיכנס באמצעות אימות טפסים.

כדי לפתור בעיה זו, אפשר אימות טפסים באמצעות יישום ה-snap-in של מסוף הניהול של AD FS (MMC) במחשב שבו מותקן העותק המקומי של Active Directory. לשם כך, בצע את הפעולות הבאות: 

1. בחלונית הניווט, אתר את **מדיניות האימות**.
2. תחת **פעולות** בחלונית הפרטים, בחר **ערוך אימות ראשי כללי**.
3. בכרטיסיה **אינטרא-נט** , בחר **אימות טפסים**.
4. בחר **אישור** (או **החל**).