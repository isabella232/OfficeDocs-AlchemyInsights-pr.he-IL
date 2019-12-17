---
title: הוספת קבוצה לאתר SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051102"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>בעיות בעת יצירה או קיבוץ של אתרים מחוברים ב-SharePoint Online

אירעו כמה בעיות נפוצות בעת יצירה או יצירה מחדש של אתר המחובר לקבוצה.

 אם מחקת קבוצה והאתר המחובר אליו וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.

הורד [SPO ניהול מעטפת](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 לקבלת מידע נוסף על תחילת התחלת עם powershell, ראה [תחילת התחלת עם מעטפת ניהול מקוונת של SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

הסר את האתר מאתרים שנמחקו באמצעות ה [-Cmdlet Remove-Spodeleאתר](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.

אם אתה יוצר אתר מחובר לקבוצה ומקבל אזהרה קבוצה אחרת עם אותו כינוי כבר קיימת, בדוק את הקבוצות הקיימות מ- [Office 365 ממרכז הניהול](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם אין עוד צורך או צור את האתר עם כינוי אחר שהוקצה.

קיימות דרכים שונות ליצירה ולשימוש בקבוצות מודרניות עם SharePoint.

באפשרותך לחבר אתרים קיימים לקבוצת Office 365. לקבלת מידע נוסף, ראה [חיבור קבוצת Office 365 המשתמשת בפני המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

כדי ליצור אתר המחובר לקבוצת Office 365, יהיה עליך ליצור אתר צוות. לקבלת מידע נוסף, ראה [יצירת אתר צוות ב-SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

