---
title: זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891296"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת

באפשרותך להשתמש בחיפוש ביומן הביקורת בתיבת מרכז התאימות של Microsoft 365 כדי להציג אירועי כלל תיבת דואר נכנס (יצירה, שינוי ומחיקה של כללי תיבת דואר נכנס).

1. בצע אחד מהשלבים הבאים:
   - בתיבת מרכז התאימות של Microsoft 365 <https://compliance.microsoft.com> at , עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://security.microsoft.com/auditlogsearch> ב- .

2. בכרטיסיה חיפוש **בדף** ביקורת, **הגדר** את ההגדרות הבאות:
   - **טווח תאריך ושעה:** בחר את טווח התאריך/שעה **בתיבות** **התחלה** וסיום.
   - **פעילויות**: בחר את הערך אחד או יותר מהערכים הבאים:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **עדכון כללי תיבת דואר נכנס מלקוח Outlook שלך**

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.**

4. בחר פעילות בתוצאות כדי לפתוח את הפרטים נשלף. מידע אודות הגדרות הכלל של תיבת הדואר הנכנס מוצג בשדה **פרמטרים.**

לקבלת מידע נוסף, [ראה קביעה אם משתמש יצר כלל תיבת דואר נכנס](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
