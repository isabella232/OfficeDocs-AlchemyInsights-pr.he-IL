---
title: שאלות אודות אופן השימוש בכלי הפריסה Office (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959684"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>שאלות אודות אופן השימוש בכלי הפריסה Office (ODT)

הורד את Office הפריסה של Microsoft ממרכז [ההורדות של Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
לאחר הורדת הקובץ, הפעל את קובץ ההפעלה לחילוץ עצמי, המכיל את קובץ ההפעלה של כלי הפריסה של Office (setup.exe) וקובץ תצורה לדוגמה (configuration.xml).
  
 **כדי לא לכלול או להסיר יישומי Microsoft 365 לארגונים ממחשבים של לקוח:**
  
בעת התקנת יישומי Microsoft 365 לארגונים, באפשרותך לא לכלול מוצרים ספציפיים. לשם כך, בצע את השלבים להתקנת Office באמצעות ODT, אך כלול את הרכיב ExcludeApp בקובץ התצורה שלך. לדוגמה, קובץ תצורה זה מתקין את כל מוצרי יישומי Microsoft 365 לארגונים למעט Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[מבט כולל על כלי Office הפריסה של](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

