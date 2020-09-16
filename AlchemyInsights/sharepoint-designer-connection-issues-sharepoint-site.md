---
title: בעיות חיבור ב-SharePoint designer
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
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727172"
---
# <a name="sharepoint-designer-connection-issues"></a>בעיות חיבור ב-SharePoint designer 

אם SharePoint designer נתקל בבעיות חיבור באתרי SharePoint, נסה את הפתרונות הנפוצים הבאים.

שלב 1: ודא ש-SharePoint designer 2013 מתעדכן באמצעות [Sharepoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ו [-2 באוגוסט 2016 עבור sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



שלב 2: נקה את קבצי המטמון המקומי:

1. סגור את SharePoint Designer 2013.

2. במחשב המקומי, הסר את כל הקבצים הנמצאים בכל אחת מהתיקיות הבאות.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. פתח את SharePoint Designer 2013 והזן שוב את החשבון כדי לראות אם הוא פועל.

שלב 3: [הפיכת אימות מודרני לזמין עבור Office 2013 במכשירי Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

שלב 4: מנהלי מערכת יצטרכו **לאפשר סקריפט מותאם אישית** בהגדרות מרכז הניהול של sharepoint כדי לאפשר את החיבור של sharepoint designer. ראה [התרה או מניעה של סקריפט מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) לקבלת מידע נוסף.


