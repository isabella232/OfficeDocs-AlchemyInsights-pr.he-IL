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
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912967"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>בעיות בעת יצירת אתר המחובר לקבוצה ב-SharePoint

1. אירעו מספר בעיות נפוצות בעת יצירה או יצירה מחדש של אתר המחובר לקבוצה.
אם מחקת קבוצה והאתר המחובר אליו וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.

   - הורד [SPO ניהול מעטפת](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - לקבלת מידע נוסף על תחילת התחלת עם Powershell, ראה [תחילת התחלת עם מעטפת ניהול מקוונת של SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - הסר את האתר מאתרים שנמחקו באמצעות ה [-Cmdlet Remove-Spodeleאתר](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell נדרש כדי למחוק לצמיתות אתרים בקבוצה.

1. אם אתה יוצר אתר מחובר לקבוצה ומקבל אזהרה: **קבוצה אחרת עם אותו כינוי כבר קיימת**, בדוק את הקבוצות הקיימות [ממרכז הניהול של Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם אין עוד צורך או צור את האתר עם כינוי אחר שהוקצה.

1. קיימות דרכים שונות ליצירה ולשימוש בקבוצות מודרניות עם SharePoint.

   - באפשרותך לחבר אתרים קיימים לקבוצת Microsoft 365. לקבלת מידע נוסף, ראה [חיבור קבוצת Microsoft 365 באמצעות ממשק המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - כדי ליצור אתר המחובר לקבוצת Microsoft 365, יהיה עליך ליצור [אתר צוות](https://admin.microsoft.com/sharepoint).
