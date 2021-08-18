---
title: הוספת קבוצה לאתר SharePoint חדש
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318125"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>בעיות נפוצות בעת יצירת אתר מחובר לקבוצה SharePoint

1. אם מחקת קבוצה ואת האתר המחובר שלה וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.

   - הורד [מעטפת ניהול SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - לקבלת מידע נוסף על תחילת העבודה עם Powershell, ראה [תחילת העבודה עם SharePoint מעטפת הניהול המקוונת](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - הסר את האתר מהאתרים שנמחקו באמצעות [cmdlet Powershell Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell נדרש כדי למחוק לצמיתות אתרי קבוצה.

1. אם אתה יוצר אתר מחובר לקבוצה ומקבל **אזהרה:** קבוצה אחרת עם אותו כינוי כבר קיימת, בדוק את הקבוצות הקיימות [מתוך מרכז הניהול של Microsoft 365.](https://admin.microsoft.com/AdminPortal/Home#/groups) כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם אין בה עוד צורך או צור את האתר עם כינוי אחר שהוקצה לו.

1. ישנן דרכים שונות ליצור קבוצות מודרניות ולהשתמש איתם SharePoint.

   - באפשרותך לחבר אתרים קיימים לקבוצה Microsoft 365 הקיימת. לקבלת מידע נוסף, [ראה התחברות קבוצה Microsoft 365 המשתמש SharePoint המשתמש.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - כדי ליצור Microsoft 365 קבוצה מחוברת, יהיה עליך ליצור [אתר צוות](https://admin.microsoft.com/sharepoint).
