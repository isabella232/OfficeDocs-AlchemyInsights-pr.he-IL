---
title: שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698059"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)

הורד את כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
לאחר הורדת הקובץ, הפעל את קובץ ההפעלה לחילוץ עצמי, המכיל את ההפעלה של כלי הפריסה של Office (setup. exe) וקובץ תצורה לדוגמה (configuration. xml).
  
 **כדי להוציא או להסיר את Microsoft 365 Apps עבור מוצרי ארגון ממחשבי לקוח:**
  
בעת התקנת Microsoft 365 Apps לארגון, באפשרותך לא לכלול מוצרים מסוימים. לשם כך, בצע את השלבים להתקנת Office באמצעות ODT, אך כלול את הרכיב הניתן לבלעדיות בקובץ התצורה שלך. לדוגמה, קובץ תצורה זה מתקין את כל יישומי Microsoft 365 עבור מוצרי ארגון פרט ל-Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[מבט כולל על הכלי לפריסת Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

