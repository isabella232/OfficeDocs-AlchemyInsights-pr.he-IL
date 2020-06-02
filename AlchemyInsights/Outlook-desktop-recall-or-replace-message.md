---
title: שולחן העבודה של Outlook מאחזר או מחליף הודעת דואר אלקטרוני
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502320"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>אחזור או החלפה של הודעת דואר אלקטרוני של Outlook

- כמנהל, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**. אין באפשרותך לאחזר הודעות ממרכז הניהול.
- **באפשרותך לאחזר הודעות שנשלחות לאנשים בארגונך בלבד**. אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אינך יכול לאחזר אותה.
- אתה יכול **רק לאחזר הודעות שנשלחו מ-Outlook 2016 במחשב**. אם משתמש שולח הודעה באמצעות Outlook for Mac או Outlook באינטרנט, אינך יכול לאחזר אותו.

כדי לאחזר או להחליף הודעת דואר אלקטרוני:

1. בחלונית התיקיות שמשמאל לחלון Outlook, בחר את התיקיה פריטים שנשלחו.
1. לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.
1. בחר בכרטיסיה **הודעה** ולאחר מכן בחר **בפעולות**  >  **אחזור הודעה זו**.
1. בחר באפשרות **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף בהודעה חדשה**ולאחר מכן בחר **באפשרות אישור**.
1. אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **בשלח**.
1. ההצלחה או הכישלון של אחזור הודעה תלויים בהגדרות הנמען ב-Outlook. לקבלת שלבים לבדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך

- אם אינך מנהל כללי, יש להוסיף את חשבונך לתפקיד ניהול התפקיד של מנהל eDiscovery או חיפוש תאימות כדי לחפש הודעות. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '. הרשאות עבור תפקידים אלה מוקצות [במרכז האבטחה והתאימות](https://go.microsoft.com/fwlink/?linkid=2083731).
- [יצור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/content-search) כדי למצוא את ההודעה שיש למחוק.
- [התחבר למרכז האבטחה והתאימות PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

אם אתה משתמש באימות מרובה גורמים, ראה [התחברות לאבטחה ולמרכז התאימות של Microsoft 365 באמצעות אימות מרובה גורמים](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).