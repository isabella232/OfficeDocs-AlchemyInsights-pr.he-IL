---
title: התקן במצב ממתין
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678481"
---
# <a name="device-in-pending-state"></a>התקן במצב ממתין

**דרישות מוקדמות**

1. אם אתה מגדיר רישומי מכשירים בפעם הראשונה, ודא שהצגת [מבוא לניהול מכשירים ב-תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) שידריך אותך לגבי אופן השגת מכשירים תחת השליטה של תכלת לספירה.
2. אם אתה מבצע רישום של מכשירים בתוך התכלת לספירה ישירות ומצרף אותם לתוך המנגינה, עליך לוודא שהגדרת את האפשרות ' שאתה מגדיר ' את האפשרות ' שאתה [מגדיר](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) את האפשרות ' והרישוי הקודם מתבצע. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)
3. ודא שאתה מורשה לבצע פעולות ב-תכלת AD ובמודעה מקומית. רק מנהל מערכת כללי בתכלת לספירה יכול לנהל הגדרות עבור רישומי מכשירים. בנוסף, אם אתה מגדיר רישומים אוטומטיים ב-Active Directory המקומי שלך, יהיה עליך להיות מנהל מערכת של Active Directory ו-AD FS (אם ישים).

תהליך ההרשמה להצטרפות היברידית תכלת מחייב מכשירים להיות ברשת הארגונית. היא פועלת גם באמצעות VPN, אך יש כמה אזהרות לכך. שמענו את הלקוחות זקוקים לסיוע בפתרון בעיות בתהליך ההרשמה להצטרפות היברידית תכלת לספירה תחת נסיבות עבודה מרוחקות.

**סביבת אימות ענן (שימוש בסינכרון hash של הסיסמה תכלת או אימות מעבר)**

זרימת רישום זו נקראת גם "Sync Join".

להלן פירוט של מה שקורה במהלך תהליך ההרשמה:

1. Windows 10 מגלה את רשומת נקודת חיבור השירות (SCP) כאשר המשתמש נכנס למכשיר.

    1. המכשיר מנסה תחילה לאחזר את פרטי הדייר מSCP בצד הלקוח ברישום [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. לקבלת מידע נוסף, ראה [מסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. אם היא נכשלת, ההתקן מקיים תקשורת עם Active Directory מקומי כדי לקבל מידע אודות הדייר מ-SCP. כדי לאמת את SCP, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)זה.

    > [!NOTE]
    > אנו ממליצים להפוך את SCP לזמין ב-Active Directory ורק באמצעות SCP בצד הלקוח לצורך אימות ראשוני.

2. Windows 10 מנסה לקיים תקשורת עם התכלת AD תחת הקשר המערכת כדי לאמת את עצמו כנגד תכלת לספירה.

    באפשרותך לאמת אם המכשיר יכול לגשת למשאבי Microsoft תחת חשבון המערכת באמצעות [קובץ ה-script של החיבור לרישום מכשירים](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 יוצר אישור בחתימה עצמית ומאחסן אותו תחת אובייקט המחשב ב-Active Directory מקומי. פעולה זו דורשת שורת המראה לבקר תחום.

4. אובייקט מכשיר המכיל אישור מסתנכרן עם התכלת לספירה באמצעות התחברות לספירה. מחזור הסינכרון מתבצע כל 30 דקות כברירת מחדל, אך תלוי בקביעת התצורה של התחברות של תכלת לספירה. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)זה.

5. בשלב זה, תוכל לראות את התקן הנושא במצב "**ממתין**" תחת מכשיר להב של הפורטל התכלת.

6. בכניסה למשתמש הבא ל-Windows 10, הרישום יושלם.

    > [!NOTE]
    > אם אתה מתחבר ל-VPN והתנתקות/הכניסה מסתיימת את קישוריות התחום, באפשרותך להפעיל את הרישום באופן ידני. כדי לעשות זאת:
    >
    > הנפק `dsregcmd /join` בקשה מקומית בבקשה למנהלי מערכת או באמצעות מרחוק דרך PSExec למחשב.
    >
    > לדוגמה: `PsExec -s \\win10client01 cmd, dsregcmd /join`

לקבלת בעיות נפוצות ברישום המכשירים של תכלת Active Directory, ראה [שאלות נפוצות אודות מכשירים](https://docs.microsoft.com/azure/active-directory/devices/faq).
