---
title: SharePoint בעיות חיבור של מעצב
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942026"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint בעיות חיבור של מעצב 

אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נסה את הפתרונות הנפוצים הבאים.

שלב 1: ודא שעדכון SharePoint Designer 2013 מתעדכן [ב- SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ובעדכון [2 באוגוסט 2016 עבור SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



שלב 2: נקה את קבצי המטמון המקומיים:

1. סגור SharePoint Designer 2013.

2. במחשב המקומי, הסר את כל הקבצים שנמצאו בכל אחת מהתיקיות הבאות.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. פתח SharePoint Designer 2013 והזן שוב את החשבון כדי לראות אם הוא פועל.

שלב 3: [הפוך אימות מודרני לזמין עבור Office 2013 במכשירי Windows .](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

שלב 4: מנהלי מערכת תצטרך לאפשר **Script** מותאם אישית בהגדרות מרכז הניהול של SharePoint כדי לאפשר את חיבור SharePoint Designer. ראה [מתן אפשרות או מניעה של קובץ Script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) מותאם אישית לקבלת מידע נוסף.


