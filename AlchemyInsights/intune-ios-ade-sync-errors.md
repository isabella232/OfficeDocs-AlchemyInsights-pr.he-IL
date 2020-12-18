---
title: שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714834"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple

"זיהינו שיש לך אסימון ADE/DEP אחד או יותר הנמצאים במצב שגיאה. עד שמצב השגיאה ייפתר עבור כל אסימון מושפע, הפונקציונליות של ADE לא תפעל באופן זהה ".

שגיאה זו עשויה להופיע במספר דרכים, כולל:

1. המכשירים עשויים שלא להסתנכרן מ-ABM/ASM כדי לכוונן
2. הקצאות של פרופילי ההרשמה עשויות להיכשל
3. המכשירים עשויים שלא להשלים את ההרשמה של ADE בהצלחה

חפש את שגיאת הסינכרון המדווחת במסוף ה-intune תחת **מכשירים > התקני הרשמה > Apple הרשמה > אסימונים** וסקור את המסמכים הבאים כדי לראות את כל התיקונים הפוטנציאליים:

[שגיאות סינכרון של ABM/ASM for iOS/iPadOS ו-macOS להרשמת מכשירים אוטומטיים](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
