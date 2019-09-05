---
title: הגבל גישה ל-SharePoint או OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750665"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>הגבל גישה ל-SharePoint או OneDrive

קיימות דרכים רבות להגבלת הגישה לשירותי SharePoint Online/OneDrive. שיטות הגבלת גישה שונות אלה מתוארות להלן. 

**הגבלת הרשאה**

ב-SharePoint Online ו-OneDrive עבור עסקים, אנו מגבילים גישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי מתן גישה לאותן קבוצות/אנשים שצריכים לגשת אליהם.

- [התאמה אישית של הרשאות עבור רשימה או ספריה של SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [התאמה אישית של הרשאות אתר SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [שינוי ההרשאות בתיקיית משנה](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [בקרת גישה ממכשירים לא מנוהלים](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

כמנהל SharePoint או מנהל כללי ב-Office 365, באפשרותך לחסום או להגביל את הגישה לתוכן SharePoint ו-OneDrive מהתקנים לא מנוהלים (אלה שאינם מחוברים ל-AD היברידי או תואמי ב-Intune).

**הגבלת מיקום רשת**

כמנהל IT, באפשרותך לשלוט בגישה למשאבי SharePoint ו-OneDrive בהתבסס על מיקומי רשת מוגדרים שבהם אתה נותן אמון. פעולה זו ידועה גם כמדיניות מבוססת מיקום. לקבלת מידע נוסף, עיין [בבקרת גישה לנתוני SharePoint Online ו-OneDrive בהתבסס על מיקום הרשת](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**הגבלת נעילת אתר** 

בתוך SharePoint Online יש לך את היכולת לנעול אוסף אתרים, כך שלאף אחד אין גישה. זה מוגדר באמצעות PowerShell ואת [מעטפת ניהול מקוונת של SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) באמצעות המאפיין [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) מדינה לוקזיט.

**הגבלת משתמשים מיצירת אתרים או אתרי מאתר**

כמנהל הכללי של SharePoint admin או Office 365, באפשרותך לאפשר למשתמשים שלך ליצור ולנהל אתרי SharePoint משלהם, לקבוע אילו אתרים הם יכולים ליצור ולציין את מיקום האתרים. לקבלת מידע נוסף, עיין [בניהול יצירת אתרים ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

