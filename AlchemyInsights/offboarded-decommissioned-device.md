---
title: בעיות בהסרת מכשיר לא מחובר או הוצא מאחסון מהמלאי של המכשיר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324445"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>בעיות בהסרת מכשיר לא מחובר או הוצא מאחסון מהמלאי של המכשיר

Microsoft Defender עבור נקודת קצה אינו מאפשר כעת הסרה ידנית של רשומת המכשיר של מכשיר לא מחובר או הוצא מהמכשיר מהמלאי של המכשיר.

למטרות אבטחה, המכשיר נשאר בפורטל כהקלטה היסטורית של עד 180 יום. עם זאת, נתוני המכשיר מטוהרים בהתאם לתקופת השמירה שתצורתה נקבעה.

**הערה:** התקן מחוץ ל- offboarded או offcommissioned עובר באופן אוטומטי למצב **לא** פעיל לאחר שבעה ימים. בנוסף, מכשירים אינם פעילים ב- 30 הימים האחרונים אינם כוללים את הנתונים המשקפים את Threat and Vulnerability Management חשיפה או את הציון המאובטח של Microsoft עבור מכשירים.
 
אם עדיין אינך מעוניין לראות מכשירים מסוימים בתצוגת מלאי מכשירים, נסה למקם תגית מכשיר כדי לסנן את המכשיר שהופסק מת התצוגה מלאי מכשיר.

לקבלת מידע נוסף, ראה:

[מכשירים לא זמינים בשירות Microsoft Defender for Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[ציון חשיפה Threat and Vulnerability Management](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[תיקון חיישנים לא בריאים ב- Microsoft Defender עבור נקודת קצה](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[כיצד להשתמש בתיוג ביעילות (חלק 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[כיצד להשתמש בתיוג ביעילות (חלק 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[כיצד להשתמש בתיוג ביעילות (חלק 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




