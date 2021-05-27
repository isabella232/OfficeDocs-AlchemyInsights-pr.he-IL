---
title: כללי הפחתת פני השטח של תקיפה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676232"
---
# <a name="attack-surface-reduction-rules"></a>כללי הפחתת פני השטח של תקיפה

אי-הכללה של קבצים או תיקיות עשויה להפחית באופן חמור את ההגנה המסופקת על-ידי כללי הפחתת פני השטח של התקיפה. ניתן להפעיל קבצים שנחסמו על-ידי כלל, ולא הדוח או אירוע. אי-הכללה חלה על כל הכללים המאפשרים אי-הכללה.

אי-הכללות של ASR משתמשות באותו תחביר אנטי-וירוס של Microsoft Defender אי-הכללות. לקבלת פרטים, ראה [קביעת תצורה ואימות של אי-הכללות עבור אנטי-וירוס של Microsoft Defender סריקות](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). כדי להימנע מבעיות, [עיין בטעויות נפוצות כדי להימנע בעת הגדרת אי-הכללות](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

לא כל כללי ASR תומכים בהכללות. כדי לאמת אם הכלל שלך תומך בהיכללות, עיין בטבלה כללי [הפחתת פני השטח של התקפה](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>כללי הפחתת פני השטח של תקיפה

שטח התקיפה של הארגון שלך כולל את כל המקומות בהם תוקף עלול לסכן מכשירים או רשתות ארגוניים. הפחתת פני השטח של התקיפה משמעה הגנה על המכשירים והרשת של הארגון, מה שמשאיר תוקפים עם פחות דרכים לביצוע תקיפות. קביעת התצורה של כללי הפחתת פני השטח של התקפה ב- Microsoft Defender עבור נקודת קצה יכולה לעזור.

לקבלת מידע נוסף, ראה:

- [מפה GUID של כלל ASR לשם](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- דרישות כללי ASR:
    - [Windows 10 Pro, גירסה 1709 ואילך](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, גירסה 1709 ואילך](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, גירסה 1803 (ערוץ חצי שנתי) ואילך](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>זהה את האי-הכללה הנכונה להחלה

1. חפש את eventID 1121 או 1122 ביומן Microsoft-Windows-Windows Defender/Operational.

1. להעריך את תרחיש הבלוק ואת ההקשר ואשר שיש לבטל חסימה של תרחיש זה.

1. קרא את הערך נתיב בפרטי האירוע, שהוא הערך המגדיר את האי-הכללה.
    - הפוך את האי-הכללה לקפדן ככל האפשר.
    - החל תו כללי כאשר יש צורך (לדוגמה, החלף משתנה משתמש).

1. החל את האי-הכללה בהתאם לצרכי הפריסה שלך. לקבלת פרטים, ראה התאמה אישית [של כללי הפחתת פני השטח של התקפה](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>אי הכללה אינה מכובדת

1. קבע אם הכלל תומך בהיכללות. לקבלת פרטים, ראה כללי [צמצום פני השטח של תקיפה](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. סקור את האי-הכללות שהוחלו ואמת עם נתוני האירוע עבור שגיאות הקלדה או תווים כלליים שלא פירטת כהלכה. לקבלת מידע נוסף, ראה [סוגי אי-הכללה נתמכים](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. אם ההשפעה של הכלל היא גבוהה מדי, שקול להעביר את הכלל (בחזרה) למצב ביקורת כדי לבצע אימות נוסף. לקבלת פרטים, ראה [בדיקת האופן שבו תכונות Microsoft Defender עבור נקודות קצה פועלות במצב ביקורת](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. אסוף נתוני תמיכה כדי לפתוח מקרה תמיכה באמצעות פקודה זו:
    
   ** MDEClientAnalyzer.cmd -v**

    לקבלת מידע נוסף, ראה [בעיות עם מחשבים ל- Microsoft Defender עבור נקודות קצה.](issues-with-onboarding-machines.md)
