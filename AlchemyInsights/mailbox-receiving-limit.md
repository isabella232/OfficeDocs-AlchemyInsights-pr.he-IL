---
title: אכיפת מגבלת קבלת תיבת דואר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315900"
---
# <a name="mailbox-receiving-limit-enforcement"></a>אכיפת מגבלת קבלת תיבת דואר

Microsoft החלה לאחרונה לאלץ את סף תיבת הדואר של 3600 הודעות לשעה. לקבלת מידע נוסף, ראה [Exchange Online מגבלות](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 תיבות דואר המקבלות יותר מ- 3600 הודעות תוך שעה ויסותו במשך 60 הדקות הבאות. 

בנוסף, מגבלת הזוגות (SRP) של השולח חוסמת הודעות שהתקבלו על-ידי Microsoft 365 דואר אלקטרוני משולח ספציפי מוחלת. אם שולח בודד שולח מעל 33% מהסף הכולל או 1200 הודעות לשעה מתגלגלת לנמען ספציפי, מגבלת ה- SRP תיתקבל, ותיבת הדואר לא תקבל עוד הודעות משולח זה. שים לב:

- מגבלה זו היא יישום להודעות דואר אלקטרוני שהתקבלו דיירים אחרים, שולחים מקומיים או שולחים באינטרנט.
- מסירת דואר אלקטרוני לתיבת הדואר חסומה במשך 60 הדקות האחרונות. 
- שולחים לתיבות דואר אלה מקבלים הודעת אי-מסירה הדוח (5.2.121 או 5.2.122) שתיבת הדואר חרג מסף המסירה המרבי. הדייר האינטרא-דייר (דואר בתוך אותו דייר) ממשיך להישלח.
- כאשר מגבלת ה- SRP מוחלת, תיבת הדואר המקבלת ממשיכה לקבל הודעות משולחים אחרים.

מנהלי מערכת יכולים לנטר את פעילות תיבת הדואר הנוכחית על-ידי הדוח ותובנות חדשות במרכז הניהול של Exchange שנקרא "Mailboxes exceeding receiving limits". תובנה זו מופיעה רק אם לדייר יש תיבות דואר פוגעות, בעוד הדוח מופיע תמיד בלוח המחוונים אך היא ריקה אלא אם דייר אינו פוגע בתיבות דואר.

לקבלת מידע נוסף אודות מגבלות קבלת תובנות, ראה תיבות דואר [החורגות מקבלת תובנות לגבי מגבלות ב- EAC החדש.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

לקבלת מידע נוסף אודות חריגה מהמגבלות הדוח, ראה תיבות דואר החורגות [ממגבלות קבלה הדוח ב- EAC החדש.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)