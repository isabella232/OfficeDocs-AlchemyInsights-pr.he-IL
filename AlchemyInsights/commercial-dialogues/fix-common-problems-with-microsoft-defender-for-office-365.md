---
title: פתרון בעיות נפוצות ב- Microsoft Defender עבור Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330061"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>פתרון בעיות נפוצות ב- Microsoft Defender עבור Office 365

להלן כמה פתרונות לבעיות נפוצות ב- Microsoft Defender עבור Office 365:

- **השהיית הודעה**:

  עיכובים במסירת דואר אלקטרוני עלולים לגרום לסריקת כספת קבצים מצורפים של הודעות. לקבלת מידע נוסף, ראה [כספת מדיניות קבצים מצורפים](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **דווח על תוצאות חיוביות או שליליות שגויות**:

  לקבלת מידע נוסף, ראה [דיווח על הודעות וקבצים ל- Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **הפיכת הגנה כספת לזמינה**:

  1. בפורטל Microsoft 365 Defender , עבור אל מדיניות שיתוף פעולה & דואר אלקטרוני & מדיניות <https://security.microsoft.com/>  \>  \>  \> **איום כללים כספת** קישורים **במקטע מדיניות.**

     כדי לעבור ישירות לדף **כספת קישורים,** השתמש <https://security.microsoft.com/safelinksv2> ב- .

  2. בדף כספת **קישורים,** בחר את המדיניות על-ידי לחיצה על שם המדיניות.
  3. בתפריט נשלף של הפרטים שמופיע, בצע אחד מהשלבים הבאים:
     - כדי להוסיף מדיניות חדשה, בחר **+ צור**. אשף יושק כדי לעזור לך להגדיר את הגדרות המדיניות שלך.
     - כדי לערוך מדיניות קיימת, בחר את המדיניות על-ידי לחיצה על שם המדיניות. בתפריט נשלף של הפרטים שמופיע, בחר **ערוך** במקטע **הגדרות הגנה.**
  4. בדף הגדרות **הגנה,** הגדר את ההגדרות הבאות:
     - הפעל את **בחר את הפעולה עבור כתובות URL לא ידועות שעלולות להיות זדוניות בהודעות**.
     - בחר **החל קישורים בטוחים על הודעות שנשלחו בתוך הארגון**.

  לקבלת מידע נוסף, [ראה הגדרת כספת קישורים ב- Microsoft Defender עבור Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
