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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553541"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)

הורד כלי הפריסה של Office דרך [מרכז ההורדות של Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
לאחר הורדת הקובץ, הפעל קובץ הפעלה לחילוץ עצמי, אשר מכיל את Office פריסת הכלי הפעלה (setup.exe) ואת קובץ התצורה לדוגמה (configuration.xml).
  
 **כדי לא לכלול או להסיר מוצרי Office 365 ProPlus ממחשבי לקוח:**
  
בעת התקנת Office 365 ProPlus, באפשרותך לא לכלול את המוצרים. לשם כך, בצע את השלבים להתקנת Office עם ODT, אך כוללות את הרכיב ExcludeApp בקובץ התצורה שלך. לדוגמה, קובץ תצורה זו מתקינה את כל מוצרי Office 365 ProPlus פרט ל- Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[מבט כולל על כלי הפריסה של Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

