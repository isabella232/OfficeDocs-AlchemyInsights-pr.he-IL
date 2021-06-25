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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117984"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>הגדרת התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני

לקבלת מידע על האפשרויות העומדות בפניך והשלבים הדרושים, ראה [כיצד להגדיר התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני באמצעות Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
אם יש לך מכשיר או יישום שהפסקת לפעול לאחרונה, הבעיות הנפוצות ביותר הן:

- **אימות שגיאות קשורות בעת שימוש בהגשת לקוח SMTP Auth** לאחרונה ביצענו כמה שינויים הקשורים לאימות SMTP. לקבלת מידע נוסף אודות פתרון בעיות, עיין בסעיף האימות שלא נכשל בפתרון בעיות במדפסות, סורקים [ויישומים של LOB](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)ששולחים דואר אלקטרוני באמצעות Microsoft 365 או Office 365.
- **אנו מקבלים רק את גירסת TLS 1.2 בעת יצירת חיבור מאובטח Office 365** אם אתה משתמש בחיבור מאובטח (TLS), ודא שהתקן היישום שלך תומך ב- TLS 1.2. לקבלת מידע נוסף, ראה [הכנת TLS 1.2 ב- Office 365 ו- Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
לקבלת בעיות ופתרונות אחרים, ראה [פתרון בעיות במדפסות, סורקים](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)ויישומים של LOB ששולחים דואר אלקטרוני באמצעות Microsoft 365 או Office 365 .

כדי לראות את המכשירים המושפעים, עבור אל [דוח לקוחות אימות SMTP](https://protection.office.com/mailflow/dashboard).

**הערה:** Exchange Online אינו מתאים לתרחישי דיוור בצובר. כדי לשלוח דואר אלקטרוני מסחרי בצובר (לדוגמה, ידיעונים של לקוחות), עליך להשתמש בספקים של ספקים חיצוני המתמחים בשירותים אלה.
