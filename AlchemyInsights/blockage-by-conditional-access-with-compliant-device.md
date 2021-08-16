---
title: אני נחסם על-ידי Access מותנת עם מכשיר תואם
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019149"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>אני נחסם על-ידי Access מותנת עם מכשיר תואם

**כלים מומלצים ביותר**

- [כלי פותר הבעיות של רישום מכשירים](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - כלי מקיף שיעזור לך לפתור את הבעיות הנפוצות ביותר ברישום מכשירים.
- [בדיקת קובץ Script של קישוריות לרישום](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) מכשירים - כלי המשמש כדי להבטיח שהתקן יוכל לגשת לנקודות הקצה של רישום מכשירים תחת חשבון המערכת.
- [Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - כלי המשמש לחפש ולנהל מכשירים מיוקלים בסביבה שלך.

להלן כמה סיבות נפוצות לכך Access מותן עלולות להיכשל עבור מכשיר תואם או  מדוע המשתמשים שלך עשויים לקבל הודעה מכאן במהלך בקשת כניסה למשאב ארגוני.

1. **ההתקן אינו נמצא במצב מכשיר נדרש עם MDM**:

ודא שהמכשיר רשום עם ספק MDM מאושר, כגון Intune, *המסומן כתואם.* לקבלת מידע נוסף אודות Intune, עיין [במסמך זה.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) לקבלת הבנה טובה יותר של תאימות מכשירים ו- Intune, ראה שימוש במדיניות תאימות כדי [להגדיר כללים עבור מכשירים שאתה מנהל באמצעות Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). אם אתה נתקל בבעיות בהרשמה של מכשיר באמצעות Intune, חפש פרטי פתרון בעיות בפתרון בעיות [בהרשמה למכשירים ב- Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). לקבלת תמיכה נוספת ב- Intune, צור בקשת תמיכה. לשם כך, בקר בדף [עזרה ותמיכה של Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **המכשיר אינו מצורף לרשת הארגונים**:

כדי לגשת למשאבים ארגוניים, המכשיר חייב להיות מחובר לרשת הארגון, באמצעות חיבור ישיר או רשת וירטואלית פרטית (VPN) וגם מחובר לרשת מקומית או ל- Azure Active Directory. כדי להצטרף למכשיר עבודה לרשת הארגון, ראה [הצטרפות למכשיר העבודה שלך לרשת של הארגון שלך.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) כדי לרשום מכשיר אישי/BYOD, [ראה רישום המכשיר האישי שלך ברשת הארגון שלך.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- כדי לאמת אם המכשיר הצטרף לרשת, באפשרותך לבצע את השלבים עבור מכשירים רשומים [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) או במכשירי [עבודה כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). כדי היקף הבעיה לקישוריות רשת של Org, פעל לפי ההנחיות הבאות:

    1. היכנס ל- Windows באמצעות החשבון שלך בעבודה או בבית הספר, לדוגמה, alain@contoso.com.
    2. התחברות לרשת של הארגון שלך באמצעות VPN או DirectAccess.
    3. לאחר שתחבר, הקש על **מקש Windows+L כדי** לנעול את המכשיר.
    4. בטל את נעילת המכשיר באמצעות החשבון שלך בעבודה או בבית הספר ולאחר מכן נסה שוב לגשת לאפליקציה או לשירות בעייתיים.

אם אתה רואה **את הודעת השגיאה לא תוכל** להגיע משם מכאן שוב, סביר שהבעיה היא במקום אחר.

3. **מערכת ההפעלה אינה נתמכת**:

ודא שאתה משתמש בגירסה נתמכת של מערכת ההפעלה, כולל:

- **Windows לקוח**: Windows 7 ואילך

- **Windows Server**: Windows Server 2008 R2 ואילך

- **macOS**: macOS X ואילך

- **Android ו- iOS**: הגירסה העדכנית ביותר של מערכות הפעלה למכשירים ניידים של Android ו- iOS

4. **דפדפן האינטרנט אינו נתמך**:

חפש דפדפנים נתמכים להלן. עבור תמיכה ב- Chrome Windows גירסאות 1703 ואילך, נדרשת Windows 10 חשבונות חדשים. עבור Edge 85+, המשתמש צריך להיות מחובר כדי להעביר כראוי את פרטי תאימות המכשיר. לקבלת פרטים נוספים, ראה [כאן](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

חפש מידע נוסף על **השלבים לא ניתן לקבל הודעה** ופתרון בעיות [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
