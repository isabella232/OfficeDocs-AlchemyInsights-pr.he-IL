---
title: Yammer בעיות רישוי
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989730"
---
# <a name="yammer-licensing-issues"></a>Yammer בעיות רישוי

כל המשתמשים חייבים להיות בעלי רשיון כדי להשתמש בשירות Yammer Enterprise, אך כברירת מחדל, Yammer אינו דורש שלמשתמשים יהיה רשיון לגשת לשירות. כאשר מנהל מערכת משנה את ההגדרה כדי לחסום Microsoft 365 משתמשים ללא Yammer, למשתמשים לא הוקצה רשיון Yammer Enterprise אין אפשרות לגשת לשירות Yammer. לקבלת מידע נוסף, ראה [ניהול Yammer משתמשים ב- Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

כאשר רשיונות מוסרים ממשתמשים, אריח Yammer אינו מוצג עוד ושירותים אחרים יכולים להשתמש בהסרת רשיונות כדי להסתיר תכונות. במקרים אחרים, תכונות עדיין יכולות להופיע אך דורשות הקצאת רשיון להפעלה.  

**הרשיון אינו מתעדכן עבור המשתמש**  

מדי פעם, למשתמש מוקצה רשיון, אך עדיין אין לו אפשרות לגשת Yammer. סביר יותר שעיכובים יתרחשו כאשר מתבצעת הקצאה של רשיון בנפח גדול. Yammer ייתכן שמשתמשים לא יעודכנו באותו סדר של רשיונות משתנים ב- Azure AD מכיוון שהמערכת פועלת באופן אסינכרוני. המתן עד 24 שעות לפני פתיחת מקרה תמיכה כדי הדוח בעיות סינכרון רשיון.  

**הקצאת רשיון בצובר**  

ניתן להקצות רשיונות דרך מרכז הניהול או Scripting של PowerShell. לקבלת מידע נוסף, [ראה הקצאת רשיונות למשתמשים](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [והקצאת רשיונות לחשבונות משתמשים באמצעות Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

התמיכה של Microsoft אינה מספקת סיוע ביצירת קבצי Script, אך תיעוד אודות Yammer רשיון זמין. לקבלת מידע נוסף, [ראה ניהול רשיונות Yammer באמצעות Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).