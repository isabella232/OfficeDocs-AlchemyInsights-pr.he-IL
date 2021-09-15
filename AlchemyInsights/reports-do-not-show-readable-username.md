---
title: דוחות במרכז הניהול של Microsoft 365 אינם מציגים שם משתמש קריא
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327815"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>דוחות במרכז הניהול של Microsoft 365 אינם מציגים שם משתמש קריא

דוחות במרכז הניהול של Microsoft 365 אינם מציגים שמות משתמש, אלא מציגים ערכים אלפא-נומריים כגון B2BC6C15BB9FCDEA71E5CD302D228CC8.

זוהי התנהגות צפויה, והיא פורסמה במרכז ההודעות (MC275344, שפורסם ב- 3 באוגוסט 2021). 

מנהלי מערכת גלובליים יכולים להחזיר שינוי זה עבור הדייר שלהם ולהציג פרטי משתמש המאפשרים זיהוי אם נוהלי הפרטיות של הארגון שלהם מאפשרים זאת. כדי להחזיר את השינוי עבור הדייר:

1. במרכז הניהול, עבור אל **הגדרות** > **הגדרות ארגון**  > [**שירותים**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ), ובחר **דוחות**. 
1. תחת **בחר כיצד להציג פרטי משתמש**, בחר **הצג פרטי משתמש הניתנים לזיהוי בדוחות**, ולאחר מכן הפעל מחדש את הדוח.