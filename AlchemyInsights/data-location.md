---
title: מיקום נתונים
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627847"
---
# <a name="data-location"></a>מיקום נתונים

באפשרותך להציג את המיקום של הדייר 365 של Office במרכז הניהול או על-ידי התחברות ל-Exchange Online דרך PowerShell.


**מרכז ניהול:**
1. היכנס [למרכז הניהול](https://admin.microsoft.com/Adminportal/Home).
2. בחר באפשרות **הגדרות** > **פרופיל ארגוני**.
3. תחת **מיקום נתונים**, בחר באפשרות **הצגת פרטים**.


**PowerShell**
1. התחבר ל-Exchange Online באמצעות Windows PowerShell.
2. בצע את ה-cmdlet ' [קבל](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) ' של הארגון כדי להציג רשימה של המאפיינים של הדייר. 
3. הבט במאפיין ' מזהה הארגון '.

כאשר יש לך את מיקום הנתונים עבור EXO ו-SPO, באפשרותך לקבוע את מיקום הנתונים עבור שירותים אחרים שבהם אתה עשוי להשתמש [מהיכן שהנתונים שלך ממוקמים](https://products.office.com/where-is-your-data-located).