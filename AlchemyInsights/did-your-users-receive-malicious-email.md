---
title: האם המשתמשים שלך קיבלו הודעת דואר אלקטרוני זדונית
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291793"
---
# <a name="did-your-users-receive-malicious-email"></a>האם המשתמשים שלך קיבלו הודעת דואר אלקטרוני זדונית?

- כעת באפשרותך לדווח על הודעת הדואר האלקטרוני הזדונית ל- Microsoft באמצעות [השליחות של מנהלי המערכת במרכז האבטחה והתאימות](https://sip.protection.office.com/reportsubmission).

הודעות שנשלחות [בשליחות של מנהלי מערכת](https://sip.protection.office.com/reportsubmission) נסרקות, והתוצאות הבאות מוצגות בתפריט הנשלף **פרטים**:

- אם היה כשל באימות הדואר האלקטרוני של השולח בעת המסירה.
- מידע על פגיעות כלשהן במדיניות שעלולות להשפיע על קביעת האבטחה של ההודעה או לעקוף אותה.
- תוצאות נטרול נוכחיות כדי לראות אם כתובות ה- URL או קבצים שכלולים בהודעה, היו זדוניים או לא.
- משוב ממדרגים

אם נמצאה עקיפה, הסקירה מחדש אמורה להסתיים תוך דקות בודדות. אם לא הייתה בעיה באימות דואר אלקטרוני או אם המסירה לא הושפעה על ידי עקיפה, המשוב של המדרגים עלול להימשך עד יום.

אם אינך מסכים עם קביעת האבטחה הסופית בנוגע להודעה, כתובת URL או קובץ (חסום לעומת לא חסום), שלח שוב את ההודעה לאחר יום למען סריקה מחדש. הסיכויים לכך שהקביעה תשתנה לאחר שליחת ההודעה שוב, גבוהים.

בינתיים, באפשרותך להסיר הודעת דואר אלקטרוני זדונית מתיבות הדואר הנכנס של המשתמשים על-ידי ביצוע ההוראות [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- לקוחות בעלי Microsoft Defender עבור Office 365 יכולים:
    - השתמש ב['סייר האיומים' כדי למצוא ולמחוק הודעת דואר אלקטרוני חשודה](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [השתמש ב'קישורים בטוחים' כדי לחסום גישה](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) לכתובת URL זדונית
    - עקוב אחר משתמשים שלחצו על כתובות URL זדוניות וניגשו אליהן: [הצג את כתובת ה- URL של דיוג ולחץ על נתוני קביעת אבטחה](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - [הפעל 'חקירה אוטומטית'](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) באופן ידני

באפשרותך גם להגן מפני כתובות URL וקבצים זדוניים על-ידי ביצוע ההוראות ב[הגנה מפני כתובות URL וקבצים זדוניים](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).