---
title: שמירת אתר או רשימה כתבנית
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109205"
---
# <a name="save-site-or-list-as-a-template"></a>שמירת אתר או רשימה כתבנית

SharePoint אתר אלה הן הגדרות בנויות מראש שעוצבו סביב צורך עסקי מסוים. לקבלת מידע נוסף, [ראה שימוש בתבניות כדי ליצור סוגים שונים של SharePoint אתרים](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

להלן כמה בעיות/פתרונות נפוצים לגבי שמירת אתר או רשימה כתבנית ב- SharePoint Online.

**לחצן שמור תבנית אתר/רשימה אינו זמין או חסר.** 

- מנהלי מערכת יצטרכו לאפשר קובץ Script מותאם אישית כדי להפוך את תכונות התבנית לזמינות. לקבלת שלבים מפורטים, דוגמאות ושיקולים, ראה מתן אפשרות [או מניעה של קובץ Script מותאם אישית.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- הפקודה 'שמור אתר כתבנית' אינה נתמכת והיא יכולה לגרום לבעיות באתרים שמשתמשים בתשתית הפרסום של SharePoint Server.


**אין אפשרות ליצור את תבנית האתר או לא לפעול כראוי**

- ייתכן שהתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ולא מופעלת. אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, לא תוכל להשתמש בתבנית האתר כדי ליצור אתר.


- בדוק אם רשימות או ספריות כלשהן חורגות מ[סף מגבלת תצוגת רשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של 5,000 פריטים, שכן חריגה זו עלולה לחסום יצירה של תבנית אתר.


- ייתכן שהמקום משתמש במשאבים רבים מדי ולכן תבנית האתר חורגת ממגבלת 50 מגה-בית (MB).


- קיימות בעיות בהצגת נתונים מרשימה שמשתמשת בעמודת חיפוש. לקבלת מידע נוסף, ראה [רשימה שנוצרה באמצעות תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב- SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


לקבלת מידע מפורט יותר אודות בעיות ופתרונות נפוצים, ראה [יצירה ושימוש בתבניות אתר.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

