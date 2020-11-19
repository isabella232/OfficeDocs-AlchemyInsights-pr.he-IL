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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353507"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>אחזור או החלפה של הודעת דואר אלקטרוני ב-Microsoft 365

- **באפשרותך לאחזר הודעות שנשלחות לאנשים בארגון שלך בלבד**. לדוגמה, אם ההודעה נשלחה לכתובת Gmail, אין באפשרותך לאחזר אותה.
- באפשרותך **לאחזר רק הודעות שנשלחו מ-Outlook עבור המחשב**. אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותו.
- כמנהל דיירים, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell** (לקבלת מידע נוסף, ראה: [חיפוש ומחיקה של הודעות דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- אין באפשרותך לאחזר הודעות ממרכז הניהול. גלול מטה אל "חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון" לקבלת מידע נוסף.

**אחזור או החלפה של הודעת דואר אלקטרוני ששלחת**

1. בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.
2. פתח את ההודעה שברצונך לאחזר. עליך ללחוץ פעמיים כדי לפתוח את ההודעה. בחירת ההודעה כך שתופיע בחלונית הקריאה לא תאפשר לך לאחזר את ההודעה.
3. בכרטיסיה הודעה, בחר **פעולות**  >  **אחזור הודעה זו**.
4. בחר **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף אותם בהודעה חדשה ולאחר** מכן בחר **אישור**.
5. אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.
6. הצלחת או כשל של הודעת אחזור תלויה בהגדרות הנמענים ב-Outlook.

לקבלת מידע נוסף, כולל כיצד לבדוק את האחזור, ראה [אחזור או החלפה של הודעת דואר אלקטרוני ששלחת](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_כדי לחפש ולמחוק הודעות דואר אלקטרוני בארגון שלך_**, הדרך הקלה ביותר היא אם אתה מנהל מערכת כללי. אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לקבוצת התפקידים של גילוי אלקטרוני Manager או לתפקיד ניהול חיפוש התאימות. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '. הרשאות לתפקידים אלה מוקצות [במרכז התאימות של אבטחה &](https://protection.office.com/).

1. [צור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.
2. [התחבר אל מרכז התאימות של אבטחה & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

אם אתה משתמש ב-Office (אימות רב-גורמי), ראה [התחברות ל-Microsoft 365 Security & מרכז התאימות באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
