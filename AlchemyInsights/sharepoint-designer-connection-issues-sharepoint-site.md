---
title: SharePoint Designer בעיות חיבור
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840552"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer בעיות חיבור 

אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נסה את הפתרונות הבאים נפוצים.

שלב 1: ודא SharePoint Designer 2013 מתעדכן עם [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [2 באוגוסט, 2016 עדכון עבור SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



שלב 2: נקה את קבצי מטמון מקומי:

1. סגור את SharePoint Designer 2013.

2. במחשב המקומי, הסר את כל הקבצים שנמצאו בכל אחת מהתיקיות הבאות.

    - Extensions\Cache שרת %APPDATA%\Microsoft\Web
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. פתח את SharePoint Designer 2013 והזן את החשבון שוב כדי לראות אם הוא פועל.

שלב 3: [להפעיל אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

שלב 4: מנהלים יהיה עליך **לאפשר קובץ Script מותאם אישית** הגדרות מרכז הניהול של SharePoint כדי לאפשר את החיבור SharePoint Designer. עיין [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) לקבלת מידע נוסף.


