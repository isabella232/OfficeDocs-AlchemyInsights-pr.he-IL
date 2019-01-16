---
title: שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291714"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="7af6a-102">שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="7af6a-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="7af6a-103">הורד כלי הפריסה של Office דרך [מרכז ההורדות של Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="7af6a-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="7af6a-104">לאחר הורדת הקובץ, הפעל קובץ הפעלה לחילוץ עצמי, אשר מכיל את Office פריסת הכלי הפעלה (setup.exe) ואת קובץ התצורה לדוגמה (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="7af6a-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="7af6a-105">**כדי לא לכלול או להסיר מוצרי Office 365 ProPlus ממחשבי לקוח:**</span><span class="sxs-lookup"><span data-stu-id="7af6a-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="7af6a-p101">בעת התקנת Office 365 ProPlus, באפשרותך לא לכלול את המוצרים. לשם כך, בצע את השלבים להתקנת Office עם ODT, אך כוללות את הרכיב ExcludeApp בקובץ התצורה שלך. לדוגמה, קובץ תצורה זו מתקינה את כל מוצרי Office 365 ProPlus פרט ל- Publisher:</span><span class="sxs-lookup"><span data-stu-id="7af6a-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="7af6a-109">מבט כולל על כלי הפריסה של Office</span><span class="sxs-lookup"><span data-stu-id="7af6a-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

