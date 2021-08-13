---
title: הגבלת גישה SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093831"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>הגבלת גישה SharePoint או OneDrive

דרכים רבות להגביל את הגישה לשירותי SharePoint/OneDrive מקוונים. שיטות הגבלת גישה שונות אלה מפורטות להלן. 

**מגבלת הרשאה**

ב SharePoint Online ו- OneDrive for Business, אנו מגבילים את הגישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי הענקת גישה לקבוצות/אנשים שיש להם גישה בלבד.

- [התאמה אישית של הרשאות עבור SharePoint או ספריה](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [התאמה אישית SharePoint הרשאות אתר](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [שינוי ההרשאות של תיקיית משנה](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [בקרת גישה ממכשירים לא מנוהלים](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

כמנהל מערכת SharePoint כללי או כמנהל מערכת כללי, באפשרותך לחסום או להגביל את הגישה לתוכן SharePoint ותוכן OneDrive ממכשירים לא מנוהלים (אלה שלא מצורפים או תואמים ל- AD היברידיים ב- Intune).

**הגבלת מיקום רשת**

כמנהל IT, באפשרותך לשלוט בגישה למשאבי SharePoint והמשאבים OneDrive בהתבסס על מיקומי רשת מוגדרים שאתה בוטח בהם. פעולה זו נקראת גם מדיניות מבוססת מיקום. לקבלת מידע נוסף, ראה [שליטה בגישה SharePoint נתונים מקוונים OneDrive בהתבסס על מיקום הרשת](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**הגבלת נעילת אתר** 

בתוך SharePoint Online יש לך את היכולת לנעול אוסף אתרים, כך שלאף אחד אין גישה. אפשרות זו מוגדרת באמצעות PowerShell [ומעטפת SharePoint Online Management באמצעות](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) [המאפיין Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**הגבלת המשתמשים ליצור אתרים או אתרי משנה**

כמנהל מערכת SharePoint מנהל מערכת כללי, באפשרותך לאפשר למשתמשים שלך ליצור ולנהל אתרי SharePoint משלהם, לקבוע אילו אתרים הם יכולים ליצור ולציין את מיקום האתרים. לקבלת מידע נוסף, ראה [ניהול יצירת אתרים ב- SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

