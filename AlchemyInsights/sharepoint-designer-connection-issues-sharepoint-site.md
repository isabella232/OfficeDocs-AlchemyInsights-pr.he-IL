---
title: רמות הרשאה של SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760694"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer בעיות חיבור 

אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נא נסה את הפתרונות הבאים נפוצים.

שלב 1: ודא SharePoint Designer מתעדכן.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer ה-Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [עדכון עבור SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

שלב 2: נקה את קבצי מטמון מקומי

- סגור את SharePoint Designer 2013.

- במחשב המקומי, לאתר את התיקיות הבאות כדי להסיר קבצים במטמון.

- לחץ על התחל, הפעלה ומחק כל הקבצים נמצא תחת כל אחד להלן מיקומים.

שרת %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

פתח את SharePoint Designer 2013 והזן את החשבון שוב כדי לראות אם הוא פועל.

שלב 3: [להפעיל אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

שלב 4: מנהלים יהיה עליך לאפשר קובץ Script מותאם אישית כדי לאפשר את החיבור SharePoint Designer.

לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


