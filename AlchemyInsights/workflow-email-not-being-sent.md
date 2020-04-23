---
title: דואר אלקטרוני של זרימת עבודה אינו נשלח
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766134"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>דואר אלקטרוני של זרימת עבודה אינו נשלח עבור רשימה או ספריה של SharePoint

1. דואר אלקטרוני מזרימות עבודה אינם נשלחים לכל המשתמשים או למשתמשים מסוימים בלבד, או שאתה רואה את השגיאה **שהודעת הדואר האלקטרוני אינה יכולה להישלח. ודא שלדואר האלקטרוני יש נמען חוקי**.

    בדוק אם המשתמש קיים בקבוצת ההרשאות ' **כל האנשים** ' (רשימת המידע של המשתמש) עבור אוסף אתרים זה.  לדוגמה, כתובת<tenant>URL ישירה<sitename>: https://. sharepoint.com/sites//_layouts/15/b. מחבר שיפגרפיד = 0

    - אם המשתמש אינו קיים, ודא שהמשתמש נחתם בעמוד. 
    - אם זהו משתמש חיצוני, ודא שההזמנה שלהם התקבלה.
    - אם המשתמש קיים בקבוצת ההרשאות, ודא שכתובת הדואר האלקטרוני נכונה.
    - אם כתובת הדואר האלקטרוני של המשתמשים אינה מוגדרת כאן, צור התראה לדוגמה עבור אותו משתמש אשר מאלץ את הסינכרון של חשבון משתמש זה מפרופילי משתמשים של SharePoint לאוסף אתרים זה.
 
2. דואר אלקטרוני מזרימות עבודה נשלחים למנהלי אוספי האתרים אך לא למשתמשים אחרים ולראות את השגיאה **HTTP אסורה ל- <span>https:</span>/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.
 

    ראה [גישה נדחתה בעת שליחת הודעת דואר אלקטרוני לקבוצת SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    כמו כן, ודא שתכונת אוסף **ההרשאות של משתמש בגישה מוגבלת של הרשאת המשתמש** אינה פעילה.


## <a name="related-topics"></a>נושאים קשורים
רוצה לנסות את Microsoft Flow ב-SharePoint Online?
- [צור זרימה](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint וזרימה](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


