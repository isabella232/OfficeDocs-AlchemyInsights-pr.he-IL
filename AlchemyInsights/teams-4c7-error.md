---
title: שגיאת Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786670"
---
# <a name="4c7-error-in-microsoft-teams"></a>שגיאת 4c7 ב- Microsoft Teams

שגיאה זו מתרחשת מאחר ש- Microsoft Teams דורש אימות טפסים. בעת פריסת Active Directory Federation Services (AD FS), אימות טפסים אינו זמין עבור האינטרא-נט כברירת מחדל. אם האימות המשולב של Windows נכשל, תתבקש להיכנס באמצעות אימות טפסים.

כדי לפתור בעיה זו, הפוך אימות טפסים לזמין באמצעות יישום ה- Snap-in AD FS Microsoft Management Console (MMC) במחשב המכיל את העותק המקומי של Active Directory. לשם כך, בצע את הפעולות הבאות: 

1. בחלונית הניווט, עבור אל **מדיניות אימות**.
2. תחת **פעולות** בחלונית הפרטים, בחר **ערוך אימות ראשי כללי.**
3. בכרטיסיה **אינטרא-נט,** בחר **אימות טפסים**.
4. בחר **אישור** (או **החל).**