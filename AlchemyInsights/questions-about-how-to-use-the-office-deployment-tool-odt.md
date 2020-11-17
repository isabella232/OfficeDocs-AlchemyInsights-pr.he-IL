---
title: שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086157"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)

הורד את כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
לאחר הורדת הקובץ, הפעלת קובץ ההפעלה לחילוץ עצמי, המכיל את קובץ ההפעלה של כלי הפריסה של Office (setupodt.exe) וקובץ תצורה לדוגמה (configuration.xml).
  
 **כדי לא לכלול או להסיר את יישומי Microsoft 365 עבור מוצרים ארגוניים ממחשבי לקוח:**
  
בעת התקנת Microsoft 365 Apps עבור enterprise, באפשרותך לכלול מוצרים ספציפיים. כדי לעשות זאת, בצע את השלבים להתקנת Office באמצעות ה-ODT, אך כלול את הרכיב ExcludeApp בקובץ התצורה. לדוגמה, קובץ תצורה זה מתקין את כל יישומי Microsoft 365 עבור מוצרי enterprise למעט Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[מבט כולל על כלי הפריסה של Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

