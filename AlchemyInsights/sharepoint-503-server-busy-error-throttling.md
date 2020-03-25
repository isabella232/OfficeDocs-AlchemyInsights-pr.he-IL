---
title: ויסות מקוונות של SharePoint
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931227"
---
# <a name="sharepoint-online-throttling"></a>ויסות מקוונות של SharePoint

**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע. אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי. במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.

לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול. אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה. עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.

**503 שרת הוא שגיאה עמוסה**

משתמשים עלולים לקבל שרת 503 הוא שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או OneDrive. 

שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint. SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online. האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים. 

לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

אם אתה סבור ששגיאה זו אינה קשורה לוויסות, באפשרותך לבדוק אם קיים תחזוקה פעילה המתרחשת בדייר שלך על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/MessageCenter).

 לבסוף, ודא שאתה מבקר בדף [הבריאות של השירות](https://portal.office.com/adminportal/home#/servicehealth) כדי לבדוק אם יש עלוני יידוע/אירועים שעשויים להתרחש.

