---
title: הוספת קבוצה לאתר SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507848"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>בעיות בעת יצירה או קבוצת אתרים ב- SharePoint Online מחובר

ישנן שתי בעיות נפוצות נתקל בעת יצירה או יצירה מחדש של קבוצת האתר מחובר.

 אם יש למחוק קבוצה ואתר מחובר ואתה מעוניין ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.

הורד [מעטפת ניהול SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 לקבלת מידע נוסף אודות תחילת העבודה עם powershell, ראה [תחילת העבודה עם מעטפת ניהול המקוונת של SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

להסיר את האתר למחוק אתרים באמצעות cmdlet powershell של [SPODeletedSite הסרה](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

אם יצירת אתר מחובר לקבוצה ולקבל אזהרה שקיימת כבר קבוצה אחרת עם כינוי זהה, בדוק את קבוצות קיימות מתוך [Office 365 ממרכז Admin](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). כדי לפתור את הבעיה, מחק קבוצה קיימת אם אין עוד צורך או ליצור את האתר עם כינוי אחר שהוקצו.

קיימות דרכים שונות כדי ליצור ולהשתמש קבוצות מודרניים עם SharePoint.

באפשרותך לחבר אתרים קיימים לקבוצת Office 365. לקבלת מידע נוסף, ראה [התחברות קבוצת Office 365 באמצעות ineterface המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

כדי ליצור אתר מחובר קבוצה של Office 365, יהיה עליך ליצור אתר צוות. לקבלת מידע נוסף, ראה [יצירת אתר צוות ב- SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

