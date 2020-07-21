---
title: משתמשים מרובים שאינם רואים תוספות ב-Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197975"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>משתמשים מרובים שאינם רואים תוספות ב-Outlook

אם בדקת את התוספות של Outlook ואף אחת מהן אינה מופיעה, כצעד הראשון לפתרון בעיות, השתמש ב **-** cmdlet ' התחבר לארגון ', כדי לבצע שאילתה על הפרמטר _Appספורצה מאופשר_ . אם השאילתה מחזירה ערך של **False**, הגדר פרמטר זה כ- **True** על-ידי שימוש ב **-cmdlet set-config** , כך שתוספות יופיעו כמצופה.

לא מומלץ לקבוע כי הפרמטר _Appספורצה מאופשר_ מוגדר כ- **False**. ערך של **שווא** דורס את כל הגדרות התפקיד הניהולי והמשתמש שלעיל ומונע הפעלה של כל היישומים החדשים על-ידי כל משתמש בארגון.

לקבלת מידע נוסף, ראה [ציון מנהלי הרשת והמשתמשים שיכולים להתקין ולנהל תוספות עבור Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).