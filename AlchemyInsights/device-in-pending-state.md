---
title: מכשיר במצב ממתין
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914004"
---
# <a name="device-in-pending-state"></a>מכשיר במצב ממתין

**דרישות מוקדמות:**

1. אם אתה מגדיר רישומי מכשירים בפעם הראשונה, ודא שסתכלת על מבוא לניהול מכשירים ב- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) שינחה אותך כיצד להשיג מכשירים תחת השליטה של Azure AD.
2. אם אתה רושם מכשירים ל- Azure AD ישירות ורושם אותם ל- Intune, יהיה עליך לוודא שתצורת [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) נקבעה [והרשיון](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) יהיה במקום הראשון.
3. ודא שאתה מורשה לבצע פעולות ב- Azure AD וב- AD מקומי. רק מנהל מערכת כללי ב- Azure AD יכול לנהל הגדרות עבור רישומי מכשירים. בנוסף, אם אתה מגדיר רישומים אוטומטיים ב- Active Directory המקומי שלך, יהיה עליך להיות מנהל מערכת של Active Directory ו- AD FS (אם רלוונטי).

תהליך הרישום ההיברידי של Azure AD מחייב שימוש במכשירים ברשת ארגונית. זה עובד גם מעל VPN, אך ישנן כמה תערות. שמענו שלקוחות זקוקים לסיוע בפתרון בעיות בתהליך רישום ההצטרפות ההיברידי של Azure AD בנסיבות עבודה מרוחקות.

**סביבת אימות ענן (באמצעות סינכרון Hash של סיסמת Azure AD או אימות מעבר)**

זרימת רישום זו נקראת גם "Sync Join".

להלן פירוט של מה שקורה במהלך תהליך הרישום:

1. Windows 10 את רשומת נקודת חיבור השירות (SCP) כאשר המשתמש נכנס למכשיר.

    1. ההתקן מנסה תחילה לאחזר פרטי דיירים מ- SCP בצד הלקוח ברישום [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. לקבלת מידע נוסף, ראה [מסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. אם הוא נכשל, המכשיר מקיים תקשורת עם Active Directory מקומי כדי לקבל מידע אודות דיירים מ- SCP. כדי לאמת את SCP, עיין [במסמך זה.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > מומלץ להפוך את SCP לפעיל ב- Active Directory ורק באמצעות SCP בצד הלקוח לאימות הראשוני.

2. Windows 10 מנסה לקיים תקשורת עם Azure AD תחת הקשר המערכת כדי לאמת את עצמה מול Azure AD.

    באפשרותך לוודא אם המכשיר יכול לגשת למשאבי Microsoft תחת חשבון המערכת באמצעות קובץ ה- [Script של קישוריות רישום מכשיר הבדיקה](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 יוצר אישור בחתימה עצמית ומאחסן אותו תחת אובייקט המחשב ב- Active Directory מקומי. פעולה זו דורשת קו ראייה לבקר תחום.

4. אובייקט התקן בעל אישור מסונכרן ל- Azure AD באמצעות Azure AD התחברות. מחזור הסינכרון הוא כל 30 דקות כברירת מחדל, אך הוא תלוי בתצורה של Azure AD התחברות. לקבלת מידע נוסף, עיין [במסמך זה.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. בשלב זה, תוכל לראות את מכשיר הנושא במצב " ממתין " תחת **להב** המכשיר של Azure Portal.

6. בכניסה הבאה של המשתמש Windows 10, הרישום יושלם.

    > [!NOTE]
    > אם אתה משתמש ב- VPN והתנתק/כניסה מסיים את קישוריות התחום, באפשרותך להפעיל את הרישום באופן ידני. לשם כך:
    >
    > הנפק `dsregcmd /join` בקשה למנהל מערכת באופן מקומי או מרחוק באמצעות PSExec למחשב שלך.
    >
    > לדוגמה: `PsExec -s \\win10client01 cmd, dsregcmd /join`

לקבלת בעיות נפוצות ברישום מכשיר Azure Active Directory, ראה שאלות [נפוצות בנושא מכשירים](https://docs.microsoft.com/azure/active-directory/devices/faq).
