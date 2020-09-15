---
title: זיהוי כתובת IP ולקוח ביומני ביקורת
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668311"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>זיהוי כתובת IP ולקוח ביומני ביקורת

כתובת ה-IP התואמת לפעילות על-ידי משתמש או מנהל של Microsoft 365 מוצגת ביומני הביקורת. פרטי הלקוח נרשמים גם הם. להלן השלבים לזיהוי מידע כזה

1. היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/).

2. עבור אל דף **Search**  >  **החיפוש ביומן ביקורת** חיפוש.

   אם אתה מעוניין בפעילות ספציפית, בחר אותה מהרשימה **פעילויות** . אם לא, כל הפעילויות יוחזרו עבור המשתמש שנבחר (הגדרת ברירת המחדל).

   **הערה**: ייתכן שפעילויות מסוימות לא יהיו זמינות בתפריט ' **פעילויות** '; עם זאת, פריטי ביקורת אלה יוחזרו אם האפשרות ' הגדרת **תוצאות עבור כל הפעילויות** ' נבחרה (הגדרת ברירת המחדל).

3. ציין את שם המשתמש בשדה **משתמשים** , בחר את טווח התאריכים המתאים עבור הפעילות ולאחר מכן לחץ על **חיפוש**.

בתוצאות, באפשרותך לראות את כתובת ה-IP של פעילות זו בחלונית התוצאות. בחר את רשומת הביקורת כדי לראות מידע מפורט **בפרטים** נשלף של (לדוגמה, לקוח, משתמש שביצע פעולה וכן הלאה).

לקבלת מידע נוסף, ראה [איתור כתובת ה-IP של המחשב המשמש לגישה לחשבון שנחשף](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
