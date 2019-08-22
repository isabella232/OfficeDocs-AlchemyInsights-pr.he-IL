---
title: זרימת דואר אלקטרוני לא נשלחת
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530875"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>זרימת דואר אלקטרוני לא נשלחת עבור SharePoint רשימה או ספריה

1. דואר אלקטרוני מתוך זרימות עבודה אינן נשלחות לכל המשתמשים או רק למשתמשים מסוימים, או שאתה רואה שאין אפשרות לשלוח את השגיאה **הודעת הדואר האלקטרוני. ודא כי הדואר האלקטרוני יש נמען חוקי**.

    בדוק אם המשתמש קיים בקבוצה הרשאות **לכל האנשים** (רשימת פרטי משתמש) עבור אוסף אתרים זה.  דגימה ישירה של כתובת URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - אם המשתמש אינו קיים, ודא שהמשתמש מחובר לתוך הדף. 
    - אם הוא משתמש חיצוני, ודא כי ההזמנה שלהם התקבלה.
    - אם המשתמש קיים בקבוצה הרשאות, ודא כי כתובת דואר אלקטרוני נכונה.
    - אם כתובת הדואר האלקטרוני של משתמשים לא מוגדר כאן, צור בדוגמה של התראה עבור משתמש זה שכופה על הסינכרון של חשבון משתמש זה מפרופילי המשתמש של SharePoint כדי באוסף אתרים זה.
 
2. דואר אלקטרוני מזרימות נשלחות המנהלים של אוספי אתרים אך לא משתמשים אחרים ולראות את השגיאה **HTTP אסור כדי <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    ראה [Access נדחתה בעת שליחת דואר אלקטרוני לקבוצת SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    כמו כן, ודא כי תכונה **מצב נעילה של הרשאת משתמש גישה מוגבלת** של אוסף אתרים אינו פעיל.


## <a name="related-topics"></a>נושאים קשורים
מעוניין לנסות זרימה Microsoft ב- SharePoint Online?
- [צור זרימה](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint וזרימה](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


