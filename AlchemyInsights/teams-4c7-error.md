---
title: Teams 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049309"
---
# <a name="4c7-error-in-microsoft-teams"></a>שגיאת 4c7 Microsoft Teams

שגיאה זו מתרחשת מאחר Microsoft Teams דורש אימות טפסים. בעת פריסת Active Directory Federation Services (AD FS), אימות טפסים אינו זמין עבור האינטרא-נט כברירת מחדל. אם Windows אימות משולב נכשל, תתבקש להיכנס באמצעות אימות טפסים.

כדי לפתור בעיה זו, הפוך אימות טפסים לזמין באמצעות יישום ה- Snap-in AD FS Microsoft Management Console (MMC) במחשב המכיל את העותק המקומי של Active Directory. לשם כך, בצע את הפעולות הבאות: 

1. בחלונית הניווט, עבור אל **מדיניות אימות**.
2. תחת **פעולות** בחלונית הפרטים, בחר **ערוך אימות ראשי כללי.**
3. בכרטיסיה **אינטרא-נט,** בחר **אימות טפסים**.
4. בחר **אישור** (או **החל).**