---
title: שולחן העבודה של Outlook מאחזר או מחליף הודעת דואר אלקטרוני
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
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663991"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>אחזור או החלפה של הודעת דואר אלקטרוני של Outlook

- כמנהל המערכת, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**. אין באפשרותך לאחזר הודעות ממרכז הניהול.
- **באפשרותך לאחזר הודעות שנשלחות לאנשים בארגון שלך בלבד**. אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אין באפשרותך לאחזר אותה.
- באפשרותך **לאחזר הודעות שנשלחו מ-Outlook 2016 במחשב PC בלבד**. אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותו.

כדי לאחזר או להחליף הודעת דואר אלקטרוני:

1. בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.
1. לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.
1. בחר בכרטיסיה **הודעה** ולאחר מכן בחר באפשרות **פעולות**  >  **אחזור הודעה זו**.
1. בחר **באפשרות** **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף אותם בהודעה חדשה**ולאחר מכן בחר אישור.
1. אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.
1. ההצלחה או הכישלון של הודעת האחזור תלויים בהגדרות הנמען ב-Outlook. לקבלת שלבים לבדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך

- אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לתפקיד ' ניהול חיפוש ' של גילוי אלקטרוני Manager או תאימות לחיפוש הודעות. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '. הרשאות עבור תפקידים אלה מוקצות [במרכז האבטחה והתאימות](https://go.microsoft.com/fwlink/?linkid=2083731).
- [צור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.
- [התחבר אל מרכז האבטחה והתאימות של PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

אם אתה משתמש באימות רב-גורמי, ראה [התחברות למרכז האבטחה והתאימות של Microsoft 365 באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).