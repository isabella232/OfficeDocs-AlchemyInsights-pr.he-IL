---
title: הוספת קבוצה לאתר SharePoint
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771204"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>בעיות בעת יצירת אתר המחובר לקבוצה ב-SharePoint

1. מספר בעיות נפוצות נתקלות בעת יצירה או יצירה מחדש של אתר המחובר לקבוצה.
אם מחקת קבוצה והאתר המחובר שלה וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.

   - הורד את [מעטפת ניהול SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - לקבלת מידע נוסף אודות תחילת העבודה עם Powershell, ראה תחילת העבודה [עם מעטפת הניהול של SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - הסר את האתר מאתרים שנמחקו באמצעות ה [-Cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell נדרש כדי למחוק לצמיתות אתרי קבוצה.

1. אם אתה יוצר אתר המחובר לקבוצה ומקבל אזהרה: **קבוצה אחרת עם אותה כינוי כבר קיימת**, בדוק את הקבוצות הקיימות מתוך [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם היא אינה נחוצה עוד או צור את האתר עם כינוי אחר מוקצה.

1. קיימות דרכים שונות ליצור ולהשתמש בקבוצות מודרניות באמצעות SharePoint.

   - באפשרותך לחבר אתרים קיימים לקבוצה של Microsoft 365. לקבלת מידע נוסף, ראה [חיבור קבוצה של Microsoft 365 באמצעות ממשק המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - כדי ליצור אתר המחובר לקבוצה של Microsoft 365, יהיה עליך ליצור [אתר צוות](https://admin.microsoft.com/sharepoint).
