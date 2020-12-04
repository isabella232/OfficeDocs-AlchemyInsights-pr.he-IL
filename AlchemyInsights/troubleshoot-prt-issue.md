---
title: פתרון בעיה ב-PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573726"
---
# <a name="troubleshoot-prt-issue"></a>פתרון בעיה ב-PRT

כדי שמכשיר כלשהו ישלים את האימות, עליו להיות רשום במלואו ובמצב טוב ולרכוש אסימון רענון ראשי (PRT).

תהליך ההרשמה להצטרפות היברידית תכלת מחייב מכשירים להיות ברשת של החברה. היא פועלת גם באמצעות VPN, אך יש כמה אזהרות לכך. שמענו שהלקוחות זקוקים לסיוע בפתרון בעיות בתהליך ההרשמה להצטרפות היברידית תכלת לספירה תחת נסיבות עבודה מרחוק. להלן פירוט של המתרחש ' מתחת למכסה המנוע ' במהלך תהליך ההרשמה.

**סביבת אימות ענן (שימוש בסינכרון hash של הסיסמה תכלת או אימות מעבר)**

זרימת רישום זו נקראת גם "Sync Join".

1. Windows 10 מגלה רשומת SCP בעת הכניסה של המשתמש למכשיר.
    1. המכשיר מנסה תחילה לאחזר את פרטי הדייר מSCP בצד הלקוח ברישום [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)זה.
    2. אם היא נכשלת, ההתקן מקיים תקשורת עם Active Directory מקומי (AD) כדי לקבל פרטי דייר מנקודת חיבור השירות (SCP). כדי לאמת את SCP, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)זה. 

> [!NOTE]
> אנו ממליצים לאפשר ל-SCP במודע ולהשתמש רק בSCP בצד הלקוח לצורך אימות ראשוני.

2. Windows 10 מנסה לקיים תקשורת עם התכלת AD תחת הקשר המערכת כדי לאמת את עצמו כנגד תכלת לספירה. באפשרותך לאמת אם המכשיר יכול לגשת למשאבי Microsoft תחת חשבון המערכת באמצעות קובץ ה-script של החיבור לרישום מכשירים.

3. Windows 10 יוצר אישור בחתימה עצמית ומאחסן אותו תחת אובייקט המחשב בהודעה מקומית. פעולה זו דורשת שורת המראה לבקר תחום.

4. אובייקט מכשיר המכיל אישור מסונכרן לכיוון התכלת לספירה דרך תכלת AD Connect. מחזור הסינכרון מתבצע כל 30 דקות כברירת מחדל, אך הדבר תלוי בקביעת התצורה של התחברות של תכלת לספירה. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)זה.

5. בשלב זה, תוכל לראות את התקן הנושא במצב "ממתין" תחת מכשיר להב של הפורטל התכלת.

6. בכניסה למשתמש הבא ל-Windows 10, הרישום יושלם. 

> [!NOTE]
> אם אתה משתמש ב-VPN ותהליך התחברות מתנתק מסיים את קישוריות התחום, באפשרותך להפעיל את הרישום באופן ידני:
 1. הנפק dsregcmd/join באופן מקומי בבקשה לניהול או באמצעות מרחוק דרך PSExec למחשב. לדוגמה, PsExec-s \\ win10client01 cmd, dsregcmd/join

 2. לקבלת פרטים נוספים על בעיות הצטרפות היברידיות, ראה [פתרון בעיות במכשירים](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
