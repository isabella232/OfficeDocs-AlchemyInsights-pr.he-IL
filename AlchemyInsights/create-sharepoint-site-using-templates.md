---
title: יצירת אתר ב-SharePoint Online
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
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732226"
---
# <a name="create-sharepoint-sites-using-templates"></a>יצירת אתרי SharePoint באמצעות תבניות

היכולת לשמור אתר כתבנית אינה נתמכת בתקשורת מודרנית או באתרי צוות. לקבלת מידע נוסף אודות השימוש בתבניות [, ראה שמירה, הורדה והעלאה של אתר SharePoint כתבנית](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

להלן כמה בעיות נפוצות/פתרונות לגבי שמירת אתר או רשימה כתבנית ב-Sharepoint Online. 

**לחצן ' שמירת אתר/תבנית רשימה ' אינו זמין או חסר**

מנהלי מערכת יצטרכו לאפשר סקריפט מותאם אישית כדי להפוך את תכונות התבנית לזמינות. לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה 

- [אפשר או מנע סקריפט מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- הפקודה ' שמור אתר כתבנית ' אינה נתמכת ועלולה לגרום לבעיות באתרים המשתמשים בתשתית הפרסום של SharePoint Server.

**לא ניתן ליצור את תבנית האתר או שאינה פועלת כהלכה**

ייתכן שלתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) והיא לא תופעל. אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, אין באפשרותך להשתמש בתבנית האתר כדי ליצור אתר.

- בדוק אם רשימות או ספריות חורגות [ממגבלת המגבלה של תצוגת הרשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של פריטים של 5000, שכן אפשרות זו חוסמת את היצירה של תבנית אתר.

- ייתכן שהאתר משתמש במשאבים רבים מדי ולכן תבנית האתר חורגת ממגבלת 50 MB.


- קיימות בעיות בהצגת נתונים מתוך רשימה המשתמשת בעמודת בדיקת מידע. לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

לקבלת מידע מפורט יותר על בעיות נפוצות ופתרונות, בדוק את [האפשרות צור ושנה תבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



