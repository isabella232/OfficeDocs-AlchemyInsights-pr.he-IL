---
title: אחזור או החלפה של הודעת דואר אלקטרוני
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024387"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>אחזור או החלפה של הודעת דואר אלקטרוני Microsoft 365

- באפשרותך **לאחזר רק הודעות הנשלחות לאנשים בארגון שלך**. לדוגמה, אם ההודעה נשלחה לכתובת Gmail, לא ניתן לאחזר אותה.
- באפשרותך **לאחזר רק הודעות שנשלחו Outlook עבור המחשב**. אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותה.
- כמנהל דייר, באפשרותך לאחזר הודעות בשם המשתמשים באמצעות **PowerShell** (לקבלת מידע נוסף, ראה: [חיפוש ומחיקה של הודעות דואר אלקטרוני).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- לא ניתן לאחזר הודעות ממרכז הניהול. גלול מטה אל "חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך" לקבלת מידע נוסף.

**אחזור או החלפה של הודעת דואר אלקטרוני ששלחת**

1. בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.
2. פתח את ההודעה שברצונך לאחזר. עליך ללחוץ פעמיים כדי לפתוח את ההודעה. בחירת ההודעה כך שהיא תופיע בחלונית הקריאה לא תאפשר לך לאחזר את ההודעה.
3. בכרטיסיה הודעה, בחר **פעולות** אחזור  >  **הודעה זו.**
4. בחר **מחק עותקים שלא נקראו של הודעה זו** או מחק עותקים שלא **נקראו והחלף בהודעה חדשה** ולאחר מכן בחר **אישור.**
5. אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.
6. ההצלחה או הכשל של אחזור הודעה תלויים בהגדרות הנמענים ב- Outlook.

לקבלת מידע נוסף, כולל אופן בדיקת האחזור, ראה [אחזור או החלפה של הודעת דואר אלקטרוני ששלחת](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***כדי לחפש ולמחוק הודעות דואר אלקטרוני בארגון*** שלך, הדרך הקלה ביותר היא אם אתה מנהל מערכת כללי. אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לקבוצת התפקידים eDiscovery Manager או לתפקיד ניהול חיפוש תאימות. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים 'ניהול ארגוני' או לתפקיד ניהול חיפוש ומחיקה. הרשאות לתפקידים אלה מוקצות במרכז האבטחה [& תאימות](https://protection.office.com/).

1. [צור חיפוש תוכן כדי](https://docs.microsoft.com/microsoft-365/compliance/content-search) למצוא את ההודעה למחיקה.
2. [התחברות ל- PowerShell & האבטחה של מרכז התאימות.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

אם אתה משתמש ב- MFA (אימות רב-גורמי), ראה התחברות כדי [Microsoft 365 אבטחה & PowerShell באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
