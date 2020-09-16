---
title: הדואר האלקטרוני של זרימת העבודה אינו נשלח
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748990"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>הדואר האלקטרוני של זרימת העבודה אינו נשלח עבור רשימה או ספריה של SharePoint

1. דואר אלקטרוני מזרימות עבודה אינו נשלח לכל המשתמשים או רק למשתמשים ספציפיים, או שאתה רואה את השגיאה **אין אפשרות לשלוח את הודעת הדואר האלקטרוני. ודא שהדואר האלקטרוני מכיל נמען חוקי**.

    בדוק אם המשתמש קיים בקבוצת ההרשאות ' **כל האנשים** ' (רשימת פרטי משתמש) עבור אוסף אתרים זה.  כתובת URL ישירה <tenant> לדוגמה: https://. sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId = 0

    - אם המשתמש אינו קיים, ודא שהמשתמש מחובר לעמוד. 
    - אם זהו משתמש חיצוני, ודא שההזמנה שלהם התקבלה.
    - אם המשתמש קיים בקבוצה הרשאות, ודא שכתובת הדואר האלקטרוני נכונה.
    - אם כתובת הדואר האלקטרוני של המשתמשים אינה מוגדרת כאן, צור התראה לדוגמה עבור משתמש זה, הכופה את הסינכרון של חשבון משתמש זה מפרופילי משתמשים של SharePoint לאוסף אתרים זה.
 
2. דואר אלקטרוני מזרימות עבודה נשלח למנהלי אוסף האתרים אך לא למשתמשים אחרים ולראות את השגיאה **HTTP אסור ל <span>-https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.
 

    ראה [Access נדחה כאשר אתה שולח הודעת דואר אלקטרוני לקבוצת SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    כמו כן, ודא שהתכונה ' אוסף אתרים ' של **' מצב נעילה ' של הרשאת משתמשים בעלת גישה מוגבלת** אינה פעילה.


## <a name="related-topics"></a>נושאים קשורים
מעוניין לנסות את Microsoft Flow ב-SharePoint Online?
- [יצירת זרימה](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ו-Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


