---
title: מחק משתמש יתום מהשרת המקומי
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198184"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>מחק משתמש יתום מהשרת המקומי

כדי להסיר משתמש יתום, בצע את הפעולות הבאות:

1. אלץ סינכרון ספריות על-ידי ביצוע ההוראות ב- [מהי זהות היברידית עם הספריה הפעילה התכלת?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. כדי לאמת את סינכרון הספריות, ראה [מהי זהות היברידית באמצעות המדריך הפעיל?](https://technet.microsoft.com/library/jj151797.aspx).

3. אם הסינכרון מתפקד כראוי אך מחיקת האובייקטים של Active Directory אינה מופצות לתכלת, הסר את האובייקט היתום באופן ידני באמצעות אחד ממודולי הספריה הבאה של הכלי הפעיל עבור יישומוני cmdlet של Windows PowerShell:

    הסר-מסולאיש קשר  
    הסר-מקבוצת מולטי  
    הסר-MsolUser

    לדוגמה, כדי להסיר john.smith@contoso.com מזהה משתמש יתום, שנוצר במקור באמצעות סינכרון ספריות, הפעל את ה-cmdlet:

    הסר-MsolUser-משתמש הJohn.Smith@Contoso.com שם