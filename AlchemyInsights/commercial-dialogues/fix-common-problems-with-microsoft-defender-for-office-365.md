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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898245"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>פתרון בעיות נפוצות ב- Microsoft Defender עבור Office 365

להלן כמה פתרונות לבעיות נפוצות ב- Microsoft Defender עבור Office 365:

- **השהיית הודעה**:

  עיכובים במסירת דואר אלקטרוני עשויים לגרום לסריקת כספת קבצים מצורפים של הודעות. לקבלת מידע נוסף, ראה [כספת מדיניות קבצים מצורפים](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **דווח על תוצאות חיוביות או שליליות שגויות**:

  לקבלת מידע נוסף, ראה [דיווח על הודעות וקבצים ל- Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **הפוך את כספת הגנה על קישור לזמינה**:

  1. בפורטל Microsoft 365 Defender , עבור אל מדיניות שיתוף פעולה & דואר אלקטרוני & כללי מדיניות איום כספת קישורים <https://security.microsoft.com/>  \>  \>  \>  **במקטע מדיניות.**

     כדי לעבור ישירות לדף **כספת קישורים,** השתמש <https://security.microsoft.com/safelinksv2> ב- .

  2. בדף כספת **קישורים,** בחר את המדיניות על-ידי לחיצה על שם המדיניות.
  3. בתפריט נשלף של הפרטים שמופיע, בצע אחד מהשלבים הבאים:
     - כדי להוסיף מדיניות חדשה, בחר **+ צור**. אשף יושק כדי לעזור לך להגדיר את הגדרות המדיניות שלך.
     - כדי לערוך מדיניות קיימת, בחר את המדיניות על-ידי לחיצה על שם המדיניות. בתפריט נשלף של הפרטים שמופיע, בחר **ערוך** במקטע **הגדרות הגנה.**
  4. בדף הגדרות **הגנה,** הגדר את ההגדרות הבאות:
     - הפעל את **בחר את הפעולה עבור כתובות URL לא ידועות שעלולות להיות זדוניות בהודעות**.
     - בחר **החל קישורים בטוחים על הודעות שנשלחו בתוך הארגון**.

  לקבלת מידע נוסף, ראה [הגדרת כספת קישורים ב- Microsoft Defender עבור Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
