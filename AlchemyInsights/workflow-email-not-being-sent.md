---
title: דואר אלקטרוני של זרימת עבודה אינו נשלח
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072521"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>דואר אלקטרוני של זרימת עבודה לא נשלח עבור SharePoint או ספריה

1. דואר אלקטרוני מזרימות עבודה אינו נשלח לכל המשתמשים או למשתמשים ספציפיים בלבד, או שאתה רואה את השגיאה לא ניתן לשלוח את הודעת הדואר האלקטרוני. ודא כי לדואר **האלקטרוני יש נמען חוקי.**

    בדוק אם המשתמש קיים בקבוצה הרשאות **'כל** האנשים' (רשימת פרטי משתמש) עבור אוסף אתרים זה.  דוגמה לכתובת URL ישירה: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - אם המשתמש אינו קיים, ודא שהמשתמש מחובר לדף. 
    - אם זהו משתמש חיצוני, ודא שההזמנה שלו התקבלה.
    - אם המשתמש קיים בקבוצת ההרשאות, ודא כי כתובת הדואר האלקטרוני נכונה.
    - אם כתובת הדואר האלקטרוני של המשתמשים אינה מוגדרת כאן, צור התראה לדוגמה עבור משתמש זה, המאלץ את הסינכרון של חשבון משתמש זה מתוך פרופילי משתמשים של SharePoint לאוסף אתרים זה.
 
2. דואר אלקטרוני מזרימות עבודה נשלח למנהלי אוסף האתרים אך לא למשתמשים אחרים ו רואה את השגיאה HTTP Forbidden to **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    ראה [Access נדחתה בעת שליחת הודעת דואר אלקטרוני לקבוצה SharePoint .](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    כמו כן, ודא **שתכונת אוסף האתרים** של מצב נעילת הרשאות משתמש גישה מוגבלת אינה פעילה.


## <a name="related-topics"></a>נושאים קשורים
רוצה לנסות את Microsoft Flow ב- SharePoint Online?
- [יצירת Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ו- Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


