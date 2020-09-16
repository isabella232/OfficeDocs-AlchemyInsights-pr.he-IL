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
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727532"
---
# <a name="save-site-or-list-as-a-template"></a>שמירת אתר או רשימה כתבנית

תבניות אתר של SharePoint מיועדות להגדרות מוגדרות מוגדרות מסביב לצרכים עסקיים מסוימים. לקבלת מידע נוסף, ראה [שימוש בתבניות כדי ליצור סוגים שונים של אתרי SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

להלן כמה בעיות נפוצות/פתרונות לגבי שמירת אתר או רשימה כתבנית ב-SharePoint Online.

**לחצן ' שמור תבנית אתר/רשימה ' אינו זמין או חסר**. 

- מנהלי מערכת יצטרכו לאפשר סקריפט מותאם אישית כדי להפוך את תכונות התבנית לזמינות. לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה [התרה או מניעה של סקריפט מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- הפקודה ' שמור אתר כתבנית ' אינה נתמכת ועלולה לגרום לבעיות באתרים המשתמשים בתשתית הפרסום של SharePoint Server.


**לא ניתן ליצור את תבנית האתר או שאינה פועלת כהלכה**

- ייתכן שלתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) והיא לא תופעל. אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, אין באפשרותך להשתמש בתבנית האתר כדי ליצור אתר.


- בדוק אם רשימות או ספריות חורגות [ממגבלת המגבלה של תצוגת הרשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של פריטים של 5000, שכן אפשרות זו חוסמת את היצירה של תבנית אתר.


- ייתכן שהאתר משתמש במשאבים רבים מדי ולכן תבנית האתר חורגת ממגבלת 50 מגה-בניות (MB).


- קיימות בעיות בהצגת נתונים מתוך רשימה המשתמשת בעמודת בדיקת מידע. לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


לקבלת מידע מפורט יותר על בעיות נפוצות ופתרונות, פנה לכאן [והשתמש בתבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

