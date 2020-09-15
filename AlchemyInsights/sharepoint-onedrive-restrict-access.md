---
title: הגבל גישה ב-SharePoint או ב-OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700456"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>הגבל גישה ב-SharePoint או ב-OneDrive

קיימות דרכים רבות להגבלת הגישה לשירותי SharePoint Online/OneDrive. שיטות הגבלת גישה שונות אלה מחולקות להלן. 

**הגבלת הרשאה**

ב-SharePoint Online וב-OneDrive for Business, אנו מגבילים את הגישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי הענקת גישה לקבוצות אלה/לאנשים שאמורים לגשת אליהם.

- [התאמה אישית של הרשאות עבור רשימה או ספריה של SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [התאמה אישית של הרשאות אתר SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [שינוי ההרשאות בתיקיית משנה](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [בקרת גישה ממכשירים לא מנוהלים](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

כמנהל SharePoint או כמנהל מערכת כללי, באפשרותך לחסום או להגביל את הגישה לתוכן של SharePoint ו-OneDrive ממכשירים לא מנוהלים (מודעות לא היברידיות מצורפות או תואמות בתוך המנגינה).

**מגבלת מיקום רשת**

כמנהל IT, באפשרותך לשלוט בגישה למשאבי SharePoint ו-OneDrive בהתבסס על מיקומי רשת מוגדרים שאתה נותן בהם אמון. פעולה זו נקראת גם מדיניות מבוססת מיקום. לקבלת מידע נוסף, ראה [שליטה בגישה לנתונים של SharePoint Online ו-OneDrive בהתבסס על מיקום ברשת](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**הגבלת נעילת אתר** 

בתוך SharePoint Online יש לך את היכולת לנעול אוסף אתרים, כך שלאף אחד אין גישה אליו. הגדרה זו מוגדרת באמצעות PowerShell [ומעטפת הניהול של SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) באמצעות המאפיין [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**הגבלת משתמשים מיצירת אתרים או אתרי משנה**

כמנהל מערכת של SharePoint או כמנהל מערכת כללי, באפשרותך לאפשר למשתמשים ליצור ולנהל אתרי SharePoint משלהם, לקבוע אילו אתרים הם יוכלו ליצור ולציין את מיקום האתרים. לקבלת מידע נוסף, ראה [ניהול יצירת אתרים ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

