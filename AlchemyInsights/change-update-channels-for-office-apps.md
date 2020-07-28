---
title: שינוי ערוצי עדכון עבור יישומי Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439388"
---
# <a name="change-update-channels-for-office-apps"></a>שינוי ערוצי עדכון עבור יישומי Office

עבור התקנות Office חדשות, השתמש בהגדרות הורדת תוכנה של Office כדי לבחור את ערוץ העדכון הרצוי ולאחר מכן התקן (או התקן מחדש) יישומי Office. לקבלת מידע נוסף, ראה [ניהול הגדרות הורדת תוכנה ב-Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**שים לב** ערוץ העדכון שנבחר באמצעות הגדרות הורדת התוכנה של Office חל על כל המשתמשים המבצעים התקנות חדשות באמצעות הפורטל O365. לקבלת מידע נוסף, ראה [הורדת והתקנה או התקנה מחדש של Microsoft 365 או Office 2019 במחשב או ב-Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

עבור התקנות Office קיימות, השתמש בכלי פריסת Office (ODT) כדי לעבור לערוץ עדכונים אחר:  

1. הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office ( setup.exe ) [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. זהה את שם הערוץ שאליו ברצונך לעבור. לקבלת מידע נוסף, ראה [אפשרויות תצורה עבור כלי הפריסה של Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. צור קובץ XML של תצורה המציין את שם הערוץ המתאים, לדוגמה update.xml .  
    קצת. <Configuration>  
    b. <Updates **ערוץ = "חודשי"** />  
    c. </Configuration>
4. משורת פקודה עם הרשאות מלאות, עבור למיקום התיקיה שבו הוא setup.exe נמצא והפעל את הפקודה הבאה:  
    קצת. setup.exe /קביעת תצורה של update.xml
5. הפעל יישום של Office (כגון Excel) ולאחר **File**מכן בחר  >  **חשבון**קובץ. במקטע פרטי מוצר, בחר באפשרות **עדכן אפשרויות**  >  **עדכון כעת**.

לקבלת מידע נוסף, ראה [כיצד להחליף ערוצי עדכון עבור יישומי Office קיימים](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

להחלפת ערוצי עדכון עבור קבוצה נבחרת של משתמשים או באמצעות מנהל התצורה (SCCM), הגדר את ההגדרה עדכן ערוץ באמצעות GPO. לקבלת מידע נוסף, ראה [מבט כולל על ערוצי העדכון של Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). לקבלת פרטים, ראה [כיצד לנהל את הערוצים של Office 365 ProPlus עבור מומחי IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) [ולנהל עדכונים ל-Microsoft 365 Apps עם מנהל התצורה של נקודות הקצה של Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).