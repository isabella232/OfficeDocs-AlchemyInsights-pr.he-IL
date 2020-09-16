---
title: בעיות רישוי של קטרת
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657277"
---
# <a name="yammer-licensing-issues"></a>בעיות רישוי של קטרת

כל המשתמשים חייבים להיות בעלי רשיון לשימוש בשירות Enterprise קטרת, אך כברירת מחדל, קטרת אינו מחייב שלמשתמשים יהיה רשיון לגשת לשירות. כאשר מנהל מערכת משנה את ההגדרה כדי לחסום את משתמשי Microsoft 365 ללא רשיונות קטרת, המשתמשים לא הקצו לרשיון של קטרת Enterprise אין גישה לשירות קטרת. לקבלת מידע נוסף, ראה [ניהול רשיונות משתמשים של קטרת ב-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

בעת הסרת רשיונות ממשתמשים, האריח של קטרת אינו מוצג עוד ושירותים אחרים יכולים להשתמש בהסרת רשיונות כדי להסתיר תכונות. במקרים אחרים, תכונות עדיין יכולות להופיע אך נדרשת הקצאת רשיון להפעלה.  

**הרשיון אינו מתעדכן עבור המשתמש**  

לעתים, למשתמש מוקצה רשיון, אך עדיין אינו מצליח לגשת ל-קטרת. סביר להניח שהעיכובים מתרחשים כאשר הקצאת רשיון המונים מתבצעת. ייתכן שמשתמשי קטרת לא יתעדכנו באותו הסדר שבו הרשיונות משתנים בתכלת לספירה מכיוון שהמערכת פועלת באופן אסינכרוני. המתן עד 24 שעות לפני פתיחת מקרה תמיכה כדי לדווח על בעיות סינכרון רשיונות.  

**הקצאת רשיון בצובר**  

ניתן להקצות רשיונות באמצעות הסקריפטים של מרכז הניהול או של PowerShell. לקבלת מידע נוסף, ראה [הקצאת רשיונות למשתמשים](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [והקצאת רשיונות לחשבונות משתמשים באמצעות Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

התמיכה של Microsoft אינה מספקת סיוע ביצירת קבצי script, אך התיעוד על הקצאת רשיון של קטרת זמין. לקבלת מידע נוסף, ראה [ניהול רשיונות קטרת באמצעות Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).