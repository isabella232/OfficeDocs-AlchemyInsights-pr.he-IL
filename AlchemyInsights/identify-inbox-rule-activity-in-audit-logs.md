---
title: זיהוי פעילות כלל של תיבת דואר נכנס ביומני ביקורת
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779052"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>זיהוי פעילות כלל של תיבת דואר נכנס ביומני ביקורת

באפשרותך להשתמש בחיפוש ביומן הביקורת במרכז התאימות של Microsoft 365 Security & כדי להציג אירועים של כללי תיבת דואר נכנס (יצירה, שינוי ומחיקה של כללי תיבת דואר נכנס).

1. היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/).

2. עבור אל דף **Search**  >  **החיפוש ביומן ביקורת** חיפוש.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך סיום** .

4. תחת **פעילויות של תיבת דואר של Exchange**, ודא שהשדה ' **פעילויות** ' מוגדר ל **-New-InboxRule יצירה/שינוי/הפעלה/ביטול של כלל תיבת דואר נכנס**.

5. לחץ על **חיפוש**.

בתוצאות, בחר רשומת ביקורת. בנשלף של הפרטים, לחץ על **מידע נוסף**. מידע אודות הגדרות הכלל של תיבת הדואר הנכנס מוצג בשדה **פרמטרים** .

לקבלת מידע נוסף, ראה [קביעה אם משתמש יצר כלל תיבת דואר נכנס](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
