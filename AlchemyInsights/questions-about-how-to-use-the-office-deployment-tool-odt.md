---
title: שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553541"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)

הורד את כלי הפריסה של Office [ממרכז ההורדות של Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
לאחר הורדת הקובץ, הפעל את קובץ ההפעלה לחילוץ עצמי, המכיל את ההפעלה של כלי הפריסה של Office (setup. exe) וקובץ תצורה לדוגמה (configuration. xml).
  
 **כדי להוציא או להסיר את מוצרי Office 365 ProPlus ממחשבי לקוח:**
  
בעת התקנת Office 365 ProPlus, באפשרותך להוציא מוצרים ספציפיים. לשם כך, בצע את השלבים להתקנת Office באמצעות ODT, אך כלול את הרכיב הניתן לבלעדיות בקובץ התצורה שלך. לדוגמה, קובץ תצורה זה מתקין את כל המוצרים של Office 365 ProPlus למעט Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[מבט כולל על הכלי לפריסת Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

