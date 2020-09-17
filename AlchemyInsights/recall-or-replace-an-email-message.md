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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799205"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>אחזור או החלפה של הודעת דואר אלקטרוני ב-Microsoft 365

- **באפשרותך לאחזר הודעות שנשלחות לאנשים בארגון שלך בלבד**. אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אין באפשרותך לאחזר אותה.
- באפשרותך **לאחזר הודעות שנשלחו מ-Outlook 2016 עבור המחשב**. אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותו.
- אם אתה מנהל מערכת, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**. אין באפשרותך לאחזר הודעות ממרכז הניהול. גלול מטה אל "חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון" לקבלת מידע נוסף.

**אחזור או החלפה של הודעת דואר אלקטרוני ששלחת**

1. בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.
2. פתח את ההודעה שברצונך לאחזר. עליך ללחוץ פעמיים כדי לפתוח את ההודעה. בחירת ההודעה כך שתופיע בחלונית הקריאה לא תאפשר לך לאחזר את ההודעה.
3. בכרטיסיה הודעה, בחר **פעולות**  >  **אחזור הודעה זו**.
4. בחר **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף אותם בהודעה חדשה ולאחר**מכן בחר **אישור**.
5. אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.
6. הצלחת או כשל של הודעת אחזור תלויה בהגדרות הנמענים ב-Outlook.

לקבלת מידע נוסף, כולל כיצד לבדוק את האחזור, ראה [אחזור או החלפה של הודעת דואר אלקטרוני ששלחת](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך*** כדי לחפש ולמחוק הודעות דואר אלקטרוני בארגון שלך, הדרך הקלה ביותר היא אם אתה מנהל מערכת כללי. אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לקבוצת התפקידים של גילוי אלקטרוני Manager או לתפקיד ניהול חיפוש התאימות. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '. הרשאות לתפקידים אלה מוקצות [במרכז התאימות אבטחה &](https://protection.office.com/).

1. [צור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.
2. [התחבר למרכז התאימות של אבטחה &-PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

אם אתה משתמש ב-Office, ראה [התחברות ל-Microsoft 365 Security Center & מרכז התאימות באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
