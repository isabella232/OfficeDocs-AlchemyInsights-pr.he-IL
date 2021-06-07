---
title: בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794007"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux

מאמר זה מנחה אותך לאורך השלבים של זיהוי בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux.

חשוב לוודא תחילה שהבעיה שבה נתקלת נפתרה בגירסה [העדכנית ביותר.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

כדי להתחיל את החקירה, ראה [פתרון בעיות ביצועים עבור Microsoft Defender עבור נקודת קצה ב- Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>אי-הכללות

אי-הכללות יכולות לעזור לצמצם בעיות ביצועים. סקור את האי-הכללות שלך לפני שתתחיל כדי שכל סיכון נוסף יהיה ידוע ותועד.

לקבלת מידע נוסף, ראה [קביעת תצורה ואמת של אי-הכללות עבור Microsoft Defender עבור נקודת קצה ב- Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

כאשר יש לך קבצים מרובים & לא לכלול אותם, והם כולם באותה נקודת טעינה, ייתכן שיהיה קל יותר לא לכלול את נקודת הטעינה. החל מהפצה 101.22.80 בפברואר, באפשרותך לא לכלול נקודת טעינה שלמה.

לדוגמה, אם /mnt/backup הוא נקודת טעינה, באפשרותך להוסיף /mnt/backup לרשימת אי-הכלולות על-ידי הפעלת פקודה זו:

`$ mdatp exclusion folder add –path /mnt/backup`

**הערה:** הוספת אי-הכללות מגדילה את הסיכון לתוכנות זדוניות שלא זוהו ויש לטפל ותטמיע איתם בדאגות.

## <a name="need-help"></a>זקוק לעזרה?

כדי לסייע לך בדרך היעילה ביותר, אסוף את נתוני האבחון לפני פתיחת מקרה תמיכה.
