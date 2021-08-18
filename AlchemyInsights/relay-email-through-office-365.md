---
title: מסירת דואר אלקטרוני באמצעות Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324363"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>הגדרת התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני

לקבלת מידע על האפשרויות העומדות בפניך והשלבים הדרושים, ראה [כיצד להגדיר התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני באמצעות Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
אם יש לך מכשיר או יישום שהפסק לאחרונה לפעול, הבעיות הנפוצות ביותר הן:

- **אימות שגיאות קשורות בעת שימוש בהגשת לקוח SMTP Auth** לאחרונה ביצענו כמה שינויים הקשורים לאימות SMTP. לקבלת מידע נוסף אודות פתרון בעיות, עיין בסעיף האימות הלא-מצליחה של פתרון בעיות במדפסות, סורקים [ויישומים של LOB](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)ששולחים דואר אלקטרוני באמצעות Microsoft 365 או Office 365.
- **אנו מקבלים רק את גירסת TLS 1.2 בעת יצירת חיבור מאובטח Office 365** אם אתה משתמש בחיבור מאובטח (TLS), ודא שהתקן היישום שלך תומך ב- TLS 1.2. לקבלת מידע נוסף, ראה [הכנת TLS 1.2 ב- Office 365 ו- Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
לקבלת בעיות ופתרונות אחרים, ראה [פתרון בעיות במדפסות, סורקים](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)ויישומים של LOB ששולחים דואר אלקטרוני באמצעות Microsoft 365 או Office 365 .

כדי לראות את המכשירים המושפעים, עבור אל [דוח לקוחות אימות SMTP](https://protection.office.com/mailflow/dashboard).

**הערה:** Exchange Online אינו מתאים לתרחישי דיוור בצובר. כדי לשלוח דואר אלקטרוני מסחרי בצובר (לדוגמה, ידיעונים של לקוחות), עליך להשתמש בספקים של ספקים חיצוני המתמחים בשירותים אלה.
