---
title: הפעלת פריסת האפליקציה של Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461869"
---
# <a name="intune-win32-app-deployment"></a>הפעלת פריסת האפליקציה של Win32

Microsoft intune מאפשרת ליישומי Win32, כולל אך לא מוגבל ל-MSI ו-. EXE שיש לפרוס במכשירי Windows 10. מנגנון הפריסה שנעשה בו שימוש דורש את הרחבת הניהול של ' שימוש ' (IME) להיות נוכח בהתקן היעד. ה-IME יותקן באופן אוטומטי כתוצאה ממטרת היעד של פריסת היישום script או win32 למשתמש/מכשיר.

יש גם קבוצה של דרישות מוקדמות שיש לעמוד בהן כדי לפרוס אפליקציות Win32 הכוללות:

- פלטפורמות נתמכות: Windows 10 גירסה 1607 ואילך (גירסאות Enterprise, Pro ו-השכלה).
- ארכיטקטורה נתמכת: x86 ו-x64.
- ניהול מכשירים: הצטרף ל-עמ מ ונרשם באופן אוטומטי (כולל תחום היברידי המצורף ומדיניות קבוצתית שנרשמו באופן אוטומטי).
- תבנית חבילת יישום:. קובץ **intunewin**  שהוכן על-ידי [כלי ההכנה של תוכן Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- מגבלות
    - גודל מרבי: 8GB.
    - ארכיטקטורה שאינה נתמכת: חימוש.

סקור את הדוקטור "[הוסף, הקצה ונטר יישום Win32 ב-Microsoft intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" לקבלת מידע הקשור לשלבים אלה.

פרטים אודות פתרון בעיות בפריסה של יישומים ב-Windows כולל יישומי Win32 ניתנים לסקירה במסמכים הבאים

- [פתרון בעיות בהתקנת יישומים](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [פתרון בעיות של יישומי Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)