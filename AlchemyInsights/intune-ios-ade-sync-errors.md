---
title: שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448923"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple

"זיהינו שיש לך אסימון ADE/DEP אחד או יותר הנמצאים במצב שגיאה. עד שמצב השגיאה ייפתר עבור כל אסימון מושפע, הפונקציונליות של ADE לא תפעל כמצופה.

שגיאה זו עשויה להופיע במספר דרכים, כולל:

1. המכשירים עשויים שלא להסתנכרן מ-ABM/ASM כדי לכוונן
2. הקצאות של פרופילי ההרשמה עשויות להיכשל
3. המכשירים עשויים שלא להשלים את ההרשמה של ADE בהצלחה

חפש את שגיאת הסינכרון המדווחת במסוף ה-intune תחת **מכשירים > התקני הרשמה > Apple הרשמת > אסימונים של תוכנית ההרשמה**.

אחת הסיבות הנפוצות ביותר לשגיאת סינכרון היא תפוגת האסימון הנוכחי. במקרים רבים, חידוש האסימון המושפע יפתור את הבעיה.

אם פג תוקף אחד או יותר מהאסימונים שלך, עיין בתיעוד הבא כדי לעזור לך לחדש אותם באופן המתאים:

[חידוש אסימון הרשמה אוטומטית של מכשירים](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

בנוסף, באפשרותך לראות את המסמכים הבאים כדי לראות תיקונים פוטנציאליים עבור שגיאות אחרות הגורמות לכשלים בסינכרון אסימונים:

[שגיאות סינכרון של ABM/ASM for iOS/iPadOS ו-macOS להרשמת מכשירים אוטומטיים](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[שגיאות סינכרון של ABM/ASM for iOS/iPadOS ו-macOS להרשמת מכשירים אוטומטיים](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
