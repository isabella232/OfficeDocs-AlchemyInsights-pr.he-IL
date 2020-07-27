---
title: משתמשים מרובים מקבלים שגיאה ב-Access נדחתה בעת הוספת תוספות ב-Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423714"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>משתמשים מרובים מקבלים שגיאה ב-Access נדחתה בעת הוספת תוספות ב-Outlook

באפשרותך לציין לאילו מנהלים בארגון שלך יש הרשאות להתקנה ולניהול של תוספות עבור Outlook. באפשרותך גם לציין לאילו משתמשים בארגון שלך יש הרשאה להתקין ולנהל תוספות לשימוש שלהם.

לקבלת פרטים, ראה [ציון המנהלים והמשתמשים שיכולים להתקין ולנהל תוספות עבור Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

כדי לוודא שהקצית בהצלחה הרשאות עבור משתמש, החלף את <Role Name> שם התפקיד לאימות והפעל את הפקודה הבאה ב-Exchange Online PowerShell:

תפקיד מקבל <Role Name> -משימות

דוגמה זו מראה לך כיצד לוודא מי הקצית הרשאות להתקנת תוספות ממאגר Office עבור הארגון.

PowerShell

-תפקיד "יישומים ביתיים של ארגון"-משתמשי הגאוטתמשתמשים

בתוצאות, בדוק את הערכים בעמודת המשתמשים האפקטיביים.

לקבלת הקצאה מפורטת של תחביר ומידע אודות פרמטרים, ראה [הקצאת משימות לניהול](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 