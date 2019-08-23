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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="5fefe-102">שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="5fefe-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="5fefe-103">הורד כלי הפריסה של Office דרך [מרכז ההורדות של Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="5fefe-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="5fefe-104">לאחר הורדת הקובץ, הפעל קובץ הפעלה לחילוץ עצמי, אשר מכיל את Office פריסת הכלי הפעלה (setup.exe) ואת קובץ התצורה לדוגמה (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="5fefe-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="5fefe-105">**כדי לא לכלול או להסיר מוצרי Office 365 ProPlus ממחשבי לקוח:**</span><span class="sxs-lookup"><span data-stu-id="5fefe-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="5fefe-106">בעת התקנת Office 365 ProPlus, באפשרותך לא לכלול את המוצרים.</span><span class="sxs-lookup"><span data-stu-id="5fefe-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="5fefe-107">לשם כך, בצע את השלבים להתקנת Office עם ODT, אך כוללות את הרכיב ExcludeApp בקובץ התצורה שלך.</span><span class="sxs-lookup"><span data-stu-id="5fefe-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="5fefe-108">לדוגמה, קובץ תצורה זו מתקינה את כל מוצרי Office 365 ProPlus פרט ל- Publisher:</span><span class="sxs-lookup"><span data-stu-id="5fefe-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="5fefe-109">מבט כולל על כלי הפריסה של Office</span><span class="sxs-lookup"><span data-stu-id="5fefe-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

