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
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093710"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>בעיות נפוצות בעת יצירת אתר מחובר לקבוצה SharePoint

1. אם מחקת קבוצה ואת האתר המחובר שלה וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.

   - הורד [מעטפת ניהול SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - לקבלת מידע נוסף אודות תחילת העבודה עם Powershell, ראה [תחילת העבודה עם מעטפת SharePoint ניהול מקוון](/powershell/module/sharepoint-online/remove-sposite).
   - הסר את האתר מהאתרים שנמחקו באמצעות [cmdlet Powershell Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell נדרש כדי למחוק לצמיתות אתרי קבוצה.

1. אם אתה יוצר אתר מחובר לקבוצה ומקבל **אזהרה:** קבוצה אחרת עם אותו כינוי כבר קיימת, בדוק את הקבוצות הקיימות מתוך [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם אין בה עוד צורך או צור את האתר עם כינוי אחר שהוקצה לו.

1. ישנן דרכים שונות ליצור קבוצות מודרניות ולהשתמש איתם SharePoint.

   - באפשרותך לחבר אתרים קיימים לקבוצה Microsoft 365. לקבלת מידע נוסף, [ראה התחברות קבוצה Microsoft 365 באמצעות SharePoint המשתמש .](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - כדי ליצור Microsoft 365 קבוצה מחוברת, תצטרך ליצור אתר [צוות](https://admin.microsoft.com/sharepoint).
