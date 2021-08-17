---
title: יצירת אתר ב- SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057967"
---
# <a name="create-sharepoint-sites-using-templates"></a>יצירת SharePoint באמצעות תבניות

היכולת לשמור אתר כתבנית אינה נתמכת עם אתרי תקשורת מודרניים או אתרי צוות. לקבלת מידע נוסף אודות השימוש בתבניות, ראה [שמירה, הורדה והעלאה של אתר SharePoint כתבנית](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

להלן כמה בעיות/פתרונות נפוצים לגבי שמירת אתר או רשימה כתבנית ב- Sharepoint Online. 

**לחצן שמור תבנית אתר/רשימה אינו זמין או חסר**

מנהלי מערכת יצטרכו לאפשר קובץ Script מותאם אישית כדי להפוך את תכונות התבנית לזמינות. לקבלת שלבים מפורטים, דוגמאות ושיקולים, ראה 

- [התרה או מניעה של קובץ Script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- הפקודה 'שמור אתר כתבנית' אינה נתמכת והיא יכולה לגרום לבעיות באתרים שמשתמשים בתשתית הפרסום של SharePoint Server.

**אין אפשרות ליצור את תבנית האתר או לא לפעול כראוי**

ייתכן שהתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ולא מופעלת. אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, לא תוכל להשתמש בתבנית האתר כדי ליצור אתר.

- בדוק אם רשימות או ספריות כלשהן חורגות מ[סף מגבלת תצוגת רשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של 5,000 פריטים, שכן חריגה זו עלולה לחסום יצירה של תבנית אתר.

- ייתכן שהאתר משתמש ביותר מדי משאבים ולכן תבנית האתר חורגת ממגבלת ה- MB 50.


- קיימות בעיות בהצגת נתונים מרשימה שמשתמשת בעמודת חיפוש. לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית לא מציגה נתונים מרשימת החיפוש הנכונה ב- SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

לקבלת מידע מפורט יותר אודות בעיות ופתרונות נפוצים, עיין [ביצירה ובשימוש בתבניות אתר.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



