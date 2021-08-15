---
title: שגיאות סינכרון של הרשמת מכשירים אוטומטיים של Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013749"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>שגיאות סינכרון של הרשמת מכשירים אוטומטיים של Apple

"זיהינו שיש לך אסימוני ADE/DEP אחד או יותר, אשר נמצאים במצב שגיאה. עד לפתרון מצב השגיאה עבור כל אסימון מושפע, הפונקציונליות של ADE לא תיפתר כצפוי.".

שגיאה זו עשויה להתבטא במספר דרכים, כולל:

1. ייתכן שהמכשירים לא יסונכרנו מ- ABM/ASM עם Intune
2. ייתכן שהקצאות פרופיל הרשמה נכשלות
3. ייתכן שהמכשירים לא ישימו את ההרשמה ל- ADE בהצלחה

בדוק את שגיאת הסינכרון המדווחת בקונסולת Intune **תחת מכשירים > הרשמה > של Apple > אסימוני תוכנית הרשמה**.

אחת הסיבות הנפוצות ביותר לשגיאה בסינכרון היא תפוגת האסימון הנוכחי. במקרים רבים, חידוש האסימון המושפע יפתור את הבעיה.

אם פג תוקפו של אחד או יותר מהאסימונים שלך, עיין בתיעוד הבא כדי לעזור לך לחדש אותם בהתאם לצורך:

[חידוש אסימון רישום אוטומטי של מכשיר](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

בנוסף, באפשרותך לראות את התיעוד הבא כדי לראות תיקון פוטנציאלי עבור שגיאות אחרות שגרמו לכשלים בסינכרון אסימון:

[שגיאות סינכרון של ABM/ASM עבור iOS/iPadOS ו- macOS אסימוני הרשמה אוטומטית של מכשירים](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[שגיאות סינכרון של ABM/ASM עבור iOS/iPadOS ו- macOS אסימוני הרשמה אוטומטית של מכשירים](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
