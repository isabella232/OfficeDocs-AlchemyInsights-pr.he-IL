---
title: יצירת אתר ב-SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770424"
---
# <a name="create-sharepoint-sites-using-templates"></a>יצירת אתרי SharePoint באמצעות תבניות

היכולת לשמור אתר כתבנית אינה נתמכת עם תקשורת מודרנית או אתרי צוות. לקבלת מידע נוסף אודות השימוש בתבניות [, ראה שמירה, הורדה וטעינה של אתר SharePoint כתבנית](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

להלן כמה בעיות/פתרונות נפוצים לגבי שמירת אתר או רשימה כתבנית ב-Sharepoint Online. 

**לחצן שמירת תבנית של אתר/רשימה אינו זמין או חסר**

מנהלי מערכת יצטרכו לאפשר Script מותאם אישית כדי להפוך את תכונות התבנית לזמינות. לקבלת שלבים מפורטים, דוגמאות ושיקולים לראות 

- [התרה או מניעה של קובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- הפקודה ' שמור אתר כתבנית ' אינה נתמכת ועלולה לגרום לבעיות באתרים המשתמשים בתשתית הפרסום של SharePoint Server.

**אין אפשרות ליצור את תבנית האתר או לא לפעול כראוי**

ייתכן שהתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ולא תפעיל אותה. אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, אין באפשרותך להשתמש בתבנית האתר כדי ליצור אתר.

- בדוק אם רשימות או ספריות מסוימות חורגות [ממגבלת הרשימה של מגבלת התצוגה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של 5000 פריטים מאחר שאפשרות זו חוסמת יצירה של תבנית אתר.

- ייתכן שהאתר משתמש במשאבים רבים מדי ולכן התבנית של האתר חורגת ממגבלת 50 MB.


- קיימות בעיות בהצגת נתונים מרשימה המשתמשת בעמודת בדיקת מידע. לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

לקבלת מידע מפורט יותר אודות בעיות ופתרונות נפוצים, נא בדוק [יצירה ושימוש בתבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



