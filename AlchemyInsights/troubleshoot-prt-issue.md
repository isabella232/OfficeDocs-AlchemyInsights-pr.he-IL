---
title: פתרון בעיות PRT
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972717"
---
# <a name="troubleshoot-prt-issue"></a>פתרון בעיות PRT

כדי שכל מכשיר ישלים את אימותו, הוא חייב להיות רשום במלואו וב במצב טוב והוא יכול להשיג אסימון רענון ראשי (PRT).

תהליך הרישום ההיברידי של Azure AD מחייב שימוש במכשירים ברשת ארגונית. זה עובד גם מעל VPN, אך ישנן כמה תערות. שמענו שלקוחות זקוקים לסיוע בפתרון בעיות בתהליך רישום ההצטרפות ההיברידי של Azure AD בנסיבות עבודה מרחוק. להלן פירוט של מה שקורה 'מתחת למכסה המנוע' במהלך תהליך הרישום.

**סביבת אימות ענן (באמצעות סינכרון Hash של סיסמת Azure AD או אימות מעבר)**

זרימת רישום זו נקראת גם "Sync Join".

1. Windows 10 מגלה רשומת SCP כאשר המשתמש נכנס למכשיר.
    1. ההתקן מנסה תחילה לאחזר פרטי דיירים מ- SCP בצד הלקוח ברישום [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. לקבלת מידע נוסף, עיין במסמך [זה.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. אם הוא נכשל, המכשיר מקיים תקשורת עם Active Directory (AD) מקומי כדי לקבל פרטי דיירים מנקודת חיבור השירות (SCP). כדי לאמת את SCP, עיין במסמך [זה.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> מומלץ להפוך את SCP ל- AD לאפשר שימוש ב- SCP בצד הלקוח רק לאימות הראשוני.

2. Windows 10 מנסה לקיים תקשורת עם Azure AD תחת הקשר המערכת כדי לאמת את עצמה מול Azure AD. באפשרותך לוודא אם המכשיר יכול לגשת למשאבי Microsoft תחת חשבון המערכת באמצעות קובץ ה- Script של קישוריות לרישום מכשיר בדיקה.

3. Windows 10 יוצר אישור בחתימה עצמית ומאחסן אותו תחת אובייקט המחשב ב- AD מקומי. פעולה זו דורשת קו ראייה לבקר תחום.

4. אובייקט התקן הכולל אישור מסונכרן ל- Azure AD באמצעות Azure AD התחברות. מחזור הסינכרון הוא כל 30 דקות כברירת מחדל, אך הוא תלוי בתצורה של Azure AD התחברות. לקבלת מידע נוסף, עיין במסמך [זה.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. בשלב זה, תוכל לראות את מכשיר הנושא במצב "ממתין" תחת להב המכשיר של Azure Portal.

6. בכניסה הבאה של המשתמש Windows 10, הרישום יושלם. 

> [!NOTE]
> אם אתה משתמש ב- VPN ותהליך התחברות לתנתק מסיים את קישוריות התחום, באפשרותך להפעיל את הרישום באופן ידני:
 1. הנפקת dsregcmd /join באופן מקומי בהנחיה למנהל מערכת או מרחוק באמצעות PSExec למחשב שלך. לדוגמה, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. לקבלת פרטים נוספים אודות בעיות צירוף היברידי, ראה [פתרון בעיות במכשירים](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
