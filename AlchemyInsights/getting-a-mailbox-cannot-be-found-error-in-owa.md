---
title: 126 לא ניתן למצוא שגיאת קבלת תיבת דואר ב- OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426663"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>קבלת תיבת דואר לא נמצאה שגיאה ב- Outlook באינטרנט?

אם אתה משתמש ב- Outlook באינטרנט  ואתה מקבל תיבת דואר לא נמצאה לשגיאה, החשבון ששימש אותך להתחברות ל- Outlook באינטרנט אינו כולל רשיון Exchange Online ולכן, לא משויכת תיבת דואר לחשבון. מנהל המערכת יכול להקצות רשיון לחשבון שלך על-ידי ביצוע השלבים הבאים:

1. פתח את [מרכז הניהול של Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) עבור אל משתמשים פעילים תחת המקטע משתמשים ובחר את המשתמש ש רואה את השגיאה.  

2. בדף המשתמש שנפתח, עבור אל  המקטע רשיונות ואפליקציות,  בחר את ערך המיקום המתאים והקצה רשיון המכיל את Exchange Online (הרחב את הרשיון כדי לראות את הפרטים שלו). כשתסיים, לחץ על **שמור שינויים.**

במקרים מסוימים, אם הרשיון כבר מוקצה לחשבון משתמש, הסרה והקצאה מחדש של הרשיון עוזרת לפתור את הבעיה ולהקצה אותה כראוי למערכת: 

- בדוק אם מנויי M365 Exchange Online (ועוד, אם יש לך) מנויים עדכניים ולא פג תוקף לאחרונה.

לאחר שנוודא שתוקף המנוי שלך לא פג ורשיון חוקי הוקצה לחשבון המשתמש, ייתכן שהרשיון ימתין עד 24 שעות, ולכן ייתכן שיהיה עליך להמתין עד שהבעיה תיפתר. לקבלת מידע נוסף, ראה [הקצאה וניהול של רשיונות](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).