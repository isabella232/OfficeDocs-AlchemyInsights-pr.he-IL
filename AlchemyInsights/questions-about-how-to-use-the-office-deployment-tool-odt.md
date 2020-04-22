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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="b33b4-102">שאלות אודות אופן השימוש בכלי הפריסה של Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="b33b4-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="b33b4-103">הורד את כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="b33b4-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="b33b4-104">לאחר הורדת הקובץ, הפעל את קובץ ההפעלה לחילוץ עצמי, המכיל את ההפעלה של כלי הפריסה של Office (setup. exe) וקובץ תצורה לדוגמה (configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="b33b4-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="b33b4-105">**כדי להוציא או להסיר את Microsoft 365 Apps עבור מוצרי ארגון ממחשבי לקוח:**</span><span class="sxs-lookup"><span data-stu-id="b33b4-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="b33b4-106">בעת התקנת Microsoft 365 Apps לארגון, באפשרותך לא לכלול מוצרים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="b33b4-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="b33b4-107">לשם כך, בצע את השלבים להתקנת Office באמצעות ODT, אך כלול את הרכיב הניתן לבלעדיות בקובץ התצורה שלך.</span><span class="sxs-lookup"><span data-stu-id="b33b4-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="b33b4-108">לדוגמה, קובץ תצורה זה מתקין את כל יישומי Microsoft 365 עבור מוצרי ארגון פרט ל-Publisher:</span><span class="sxs-lookup"><span data-stu-id="b33b4-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="b33b4-109">מבט כולל על הכלי לפריסת Office</span><span class="sxs-lookup"><span data-stu-id="b33b4-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

