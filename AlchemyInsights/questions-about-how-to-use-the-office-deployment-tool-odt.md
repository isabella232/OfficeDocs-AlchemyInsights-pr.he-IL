---
title: שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790333"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)

הורד את כלי הפריסה של Office ממרכז [ההורדות של Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
לאחר הורדת הקובץ, הפעל את קובץ ההפעלה לחילוץ עצמי, המכיל את קובץ ההפעלה של כלי הפריסה של Office (setup.exe) וקובץ תצורה לדוגמה (configuration.xml).
  
 **כדי לא לכלול או להסיר יישומי Microsoft 365 עבור מוצרים ארגוניים מחשבי לקוח:**
  
בעת התקנת יישומי Microsoft 365 עבור הארגון, באפשרותך לא לכלול מוצרים ספציפיים. לשם כך, בצע את השלבים להתקנת Office עם ODT, אך כלול את הרכיב ExcludeApp בקובץ התצורה שלך. לדוגמה, קובץ תצורה זה מתקין את כל יישומי Microsoft 365 עבור מוצרים ארגוניים למעט Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[מבט כולל על כלי הפריסה של Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

