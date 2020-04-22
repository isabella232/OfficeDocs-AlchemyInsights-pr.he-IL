---
title: זיהוי כתובת IP ולקוח ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716389"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>זיהוי כתובת IP ולקוח ביומני ביקורת

כתובת ה-IP התואמת לפעילות על-ידי משתמש של Microsoft 365 או מנהל מערכת מוצגת ביומני ביקורת. מידע הלקוח נרשם גם הוא. להלן השלבים לזיהוי מידע שכזה

1. היכנס ל- [Microsoft 365 האבטחה _ אמפר _ מרכז התאימות](https://protection.office.com/).

2. עבור אל דף **Search** > **החיפוש של יומן ביקורת** חיפוש.

   אם אתה מעוניין בפעילות מסוימת, בחר אותה מתוך רשימת **הפעילויות** . אם לא, כל הפעילויות יוחזרו עבור המשתמש הנבחר (הגדרת ברירת המחדל).

   **הערה**: ייתכן שפעילויות מסוימות לא יהיו זמינות בתפריט ' **פעילויות** '; עם זאת, פריטי ביקורת אלה יוחזרו אם האפשרות **הצג תוצאות עבור כל הפעילויות** נבחרה (הגדרת ברירת המחדל).

3. ציין את שם המשתמש בשדה **Users** , בחר את טווח התאריכים המתאים עבור הפעילות ולאחר מכן לחץ על **חיפוש**.

בתוצאות, באפשרותך לראות את כתובת ה-IP עבור פעילות זו בחלונית התוצאות. בחר ברשומת הביקורת כדי לראות מידע מפורט בתפריט **הפרטים** (לדוגמה, לקוח, משתמש שביצע פעולה וכו ').

לקבלת מידע נוסף, ראה [איתור כתובת ה-IP של המחשב המשמש לקבלת גישה לחשבון שנפרץ](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
