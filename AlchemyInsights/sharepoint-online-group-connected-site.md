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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719483"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>צור קבוצת אתר מחוברים ב- SharePoint Online

<p><strong>ישנן שתי בעיות נפוצות נתקל בעת יצירה או יצירה מחדש של קבוצת האתר מחובר.&nbsp;</strong></p>  <p>1.אם יש למחוק קבוצה ואתר מחובר ואתה מעוניין ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.</p>  <ul>  <li>הורדת <a title="מעטפת ניהול SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">מעטפת ניהול SPO</a> - לקבלת מידע נוסף אודות תחילת העבודה עם powershell, ראה <a title="תחילת העבודה עם מעטפת ניהול המקוונת של SharePoint" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">תחילת העבודה עם מעטפת ניהול המקוונת של SharePoint</a>. <br /><br /></li>  <li>הסר את האתר מלהשתמש למחוק אתרים <a title="SPODeletedSite הסרה" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">הסר-SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>אם יצירת אתר מחובר לקבוצה ולקבל אזהרה <strong>'קבוצה אחרת עם כינוי זהה כבר קיים'</strong>, בדוק את הקבוצות הקיימות <a title="Office 365 ממרכז Admin" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 ממרכז ניהול</a>. כדי לפתור את הבעיה, מחק קבוצה קיימת אם אין עוד צורך או ליצור את האתר עם כינוי אחר שהוקצו.&nbsp;</p>  <p><strong>קיימות דרכים שונות כדי ליצור ולהשתמש קבוצות מודרניים עם SharePoint.&nbsp;</strong></p>  <ol>  <li>באפשרותך לחבר אתרים קיימים לקבוצת Office 365. לקבלת מידע נוסף, ראה <a title="להתחבר ineterface המשתמש של SharePoint באמצעות קבוצת Office 365" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">חבר קבוצת Office 365 ineterface המשתמש של SharePoint באמצעות</a>.</li>  <li>כדי ליצור אתר מחובר קבוצה של Office 365, יהיה עליך ליצור אתר צוות. לקבלת מידע נוסף, ראה <a title="ליצור אתר צוות ב- SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">צור אתר הצוות ב- SharePoint.</a></li>  </ol>

