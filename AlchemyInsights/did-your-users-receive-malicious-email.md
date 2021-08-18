---
title: האם המשתמשים שלך קיבלו הודעת דואר אלקטרוני זדונית
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326671"
---
# <a name="did-your-users-receive-malicious-email"></a>האם המשתמשים שלך קיבלו הודעת דואר אלקטרוני זדונית?

כעת באפשרותך הדוח הודעת הדואר האלקטרוני הזדונית ל- Microsoft [באמצעות הגשות בפורטל Microsoft 365 Defender .](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

הודעות הנשלחות בהפניות [למנהלי מערכת](https://security.microsoft.com/reportsubmission?viewid=admin) נסרקים, והתוצאות הבאות מוצגות בתצוגה הנשלחת של הפירוט:

- אם היה כשל באימות הדואר האלקטרוני של השולח בעת המסירה.
- מידע על פגיעות כלשהן במדיניות שעלולות להשפיע על קביעת האבטחה של ההודעה או לעקוף אותה.
- תוצאות נטרול נוכחיות כדי לראות אם כתובות ה- URL או קבצים שכלולים בהודעה, היו זדוניים או לא.
- משוב ממדרגים

אם נמצאה עקיפה, הסקירה מחדש אמורה להסתיים תוך דקות בודדות. אם לא הייתה בעיה באימות דואר אלקטרוני או אם המסירה לא הושפעה על ידי עקיפה, המשוב של המדרגים עלול להימשך עד יום.

אם אינך מסכים עם קביעת האבטחה הסופית בנוגע להודעה, כתובת URL או קובץ (חסום לעומת לא חסום), שלח שוב את ההודעה לאחר יום למען סריקה מחדש. הסיכויים לכך שהקביעה תשתנה לאחר שליחת ההודעה שוב, גבוהים.

בינתיים, באפשרותך להסיר הודעת דואר אלקטרוני זדונית מתיבות הדואר הנכנס של המשתמשים על-ידי ביצוע ההוראות [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- לקוחות בעלי Microsoft Defender עבור Office 365 יכולים:
  - שימוש [בסייר האיומים כדי לחפש ולמחוק דואר אלקטרוני חשוד](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [שימוש כספת קישורים כדי לחסום גישה לכתובת](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) URL זדונית
  - עקוב אחר משתמשים שלחיצות ולגשת לכתובות URL זדוניות: הצגת כתובת [URL של](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)דיוג ולחץ על נתוני פסק דין  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - הפעלה ידנית [של חקירה אוטומטית](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

באפשרותך גם להגן מפני כתובות URL וקבצים זדוניים על-ידי ביצוע ההוראות ב[הגנה מפני כתובות URL וקבצים זדוניים](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
