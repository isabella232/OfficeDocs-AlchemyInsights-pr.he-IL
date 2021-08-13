---
title: Outlook אחזור או החלפה של הודעת דואר אלקטרוני בשולחן העבודה
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918396"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>אחזור או החלפה של הודעת Outlook דואר אלקטרוני

- כמנהל המערכת, באפשרותך **לאחזר הודעות בשם משתמשים המשתמשים ב- PowerShell**. לא ניתן לאחזר הודעות ממרכז הניהול.
- באפשרותך **לאחזר רק הודעות הנשלחות לאנשים בארגון שלך**. אם ההודעה נשלחה לכתובת Gmail, לדוגמה, לא ניתן לאחזר אותה.
- באפשרותך **לאחזר רק הודעות שנשלחו Outlook 2016 במחשב .** אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותה.

כדי לאחזר או להחליף הודעת דואר אלקטרוני:

1. בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.
1. לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.
1. בחר את **הכרטיסיה הודעה** ולאחר מכן בחר **פעולות**  >  **אחזור הודעה זו.**
1. בחר **מחק עותקים שלא נקראו של הודעה זו** או מחק עותקים שלא **נקראו והחלף בהודעה חדשה** ולאחר מכן בחר **אישור.**
1. אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.
1. ההצלחה או הכשל של אחזור הודעה תלויים בהגדרות הנמען Outlook. לקבלת שלבים ל בדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך

- אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לתפקיד מנהל גילוי אלקטרוני או לתפקיד ניהול חיפוש תאימות כדי לחפש הודעות. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים 'ניהול ארגוני' או לתפקיד ניהול חיפוש ומחיקה. הרשאות עבור תפקידים אלה מוקצות במרכז האבטחה [והתאימות.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [צור חיפוש תוכן כדי](https://docs.microsoft.com/microsoft-365/compliance/content-search) למצוא את ההודעה למחיקה.
- [התחברות ל- PowerShell של מרכז האבטחה והתאימות.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

אם אתה משתמש באימות רב-גורמי, ראה התחברות כדי Microsoft 365 PowerShell של מרכז האבטחה [והתאימות באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).