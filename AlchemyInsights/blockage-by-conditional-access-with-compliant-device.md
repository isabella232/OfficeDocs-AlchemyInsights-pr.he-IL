---
title: אני נחסם על-ידי גישה מותנית עם התקן תואם
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035994"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>אני נחסם על-ידי גישה מותנית עם התקן תואם

**כלים מומלצים במיוחד**

- [כלי פותר בעיות רישום המכשירים](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -כלי מקיף שעוזר לפתור בעיות ברישום המכשירים הנפוצים ביותר.
- [בדיקת קובץ script של קישוריות לרישום מכשירים](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -כלי המשמש כדי להבטיח שההתקן יוכל לגשת לנקודות קצה של רישום מכשירים תחת חשבון המערכת.
- [קובץ Script לניקוי התקן תכלת](https://github.com/mzmaili/AzureADDeviceCleanup) -כלי המשמש לחיפוש ולניהול של מכשירים ישנים בסביבה שלך.

להלן כמה סיבות נפוצות לכך שגישה מותנית עשויה להיכשל עבור מכשיר תואם או מדוע ייתכן **שהמשתמשים** שלך מקבלים את ההודעה במהלך בקשת כניסה למשאב ארגוני.

1. **המכשיר אינו נמצא במצב התקן נדרש עם MDM**:

ודא שההתקן נרשם עם ספק MDM מאושר, כגון ' שלחן ' *ומסומן כתואם*. לקבלת מידע נוסף אודות המנגינה, ראה [מסמך](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)זה. לקבלת הבנה טובה יותר של תאימות מכשירים וכוונון, ראה [שימוש במדיניות תאימות כדי להגדיר כללים עבור מכשירים שאתה מנהל באמצעות ' כוונון](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)'. אם אתה נתקל בבעיות ברישום מכשיר באמצעות ' כוונון ', מצא את פרטי פתרון הבעיות [בפתרון בעיות בהרשמת מכשירים ב-Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). לקבלת תמיכה נוספת, צור בקשה לתמיכה. כדי לעשות זאת, בקר [בדף העזרה והתמיכה של כוונון](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **המכשיר אינו מצורף לרשת הארגונים**:

כדי לגשת למשאבים ארגוניים, המכשיר צריך להיות מחובר לרשת של הארגון, באמצעות חיבור ישיר או רשת וירטואלית פרטית (VPN), וכן הצטרפות למדריך הכתובות המקומי או התכלת של Active Directory. כדי להצטרף להתקן עבודה לרשת הארגונית, ראה [הצטרפות למכשיר העבודה שלך לרשת של הארגון שלך](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). כדי לרשום התקן אישי/BYOD, ראה [רישום המכשיר האישי שלך ברשת של הארגון](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)שלך.

- כדי לאמת אם המכשיר הצטרף לרשת, באפשרותך לבצע את השלבים עבור התקנים רשומים [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) או מכשירי עבודה [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). כדי להרחיב את הבעיה לקישוריות רשת ארגונית, בצע את ההנחיות הבאות:

    1. היכנס ל-Windows באמצעות החשבון שלך בעבודה או בבית הספר, לדוגמה, alain@contoso.com.
    2. התחבר לרשת של הארגון שלך דרך VPN או DirectAccess.
    3. לאחר שאתה מחובר, הקש על **מקש סמל Windows + L** כדי לנעול את המכשיר.
    4. בטל את נעילת המכשיר באמצעות החשבון שלך בעבודה או בבית הספר ולאחר מכן נסה שוב לגשת ליישום או לשירות הבעייתי.

אם אתה רואה את ההודעה **לא ניתן להגיע שוב מהודעת השגיאה הבאה** , הבעיה עשויה להיות במקום אחר.

3. **מערכת ההפעלה אינה נתמכת**:

ודא שאתה מפעיל גירסה נתמכת של מערכת ההפעלה, כולל:

- **לקוח windows**: windows 7 ואילך

- **Windows server**: windows Server 2008 R2 ואילך

- **macOS**: macos X ואילך

- **Android ו-ios**: הגירסה העדכנית ביותר של android ו-ios מערכות הפעלה ניידות

4. **דפדפן אינטרנט אינו נתמך**:

חפש בדפדפנים נתמכים להלן. עבור תמיכה ב-Chrome עם Windows 1703 וגירסאות מתקדמות יותר, נדרשת סיומת של Windows 10 חשבונות. עבור Edge 85 +, המשתמש צריך להיות מחובר כדי להעביר כהלכה את מידע תאימות המכשירים. לקבלת פרטים נוספים, ראה [כאן](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, כוונון דפדפן מנוהל, Safari
- **Android**: **Microsoft Edge**: כוונון דפדפן מנוהל, כרום
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

חפש מידע נוסף בנושא **אין באפשרותך לקבל** את ההודעה ולפתור את השלבים [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
