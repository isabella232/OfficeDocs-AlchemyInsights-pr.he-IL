---
title: 'זהה filename הוא הטוב ביותר [כלל #-תיאור]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697131"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0a18b-102">נדרש אלכימיה כותרת H1, H2 של אינם פועלים.</span><span class="sxs-lookup"><span data-stu-id="0a18b-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="0a18b-103">ושיטות עבודה מומלצות הנחיות לעריכת אלכימיה:</span><span class="sxs-lookup"><span data-stu-id="0a18b-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0a18b-p101">**לא לקנן תובנות אלכימיה בתיקיות**- פעולה זו תנתק את מבנה ה-url. אנו מביט לתוך תיקון זה.</span><span class="sxs-lookup"><span data-stu-id="0a18b-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="0a18b-106">הקבצים בתיקיה **AlchemyInsights** צריך להיות מזהה כלל ושם כלל מתוך [פורטל השותפים אלכימיה של](https://alchemyportal.azurewebsites.net) שם הקובץ.</span><span class="sxs-lookup"><span data-stu-id="0a18b-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="0a18b-p102">לדוגמה ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="0a18b-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="0a18b-p103">השתמש את המטה-נתונים בחלק העליון של קובץ זה כתבנית שלך. דבר נוסף נדרש.</span><span class="sxs-lookup"><span data-stu-id="0a18b-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="0a18b-111">[פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net), נווט למטה למקטע **הכותרת תובנות לקוח:** ושימוש המצביעים בתור התחלה עבור כותרת H1 שלך לקבלת תובנות.</span><span class="sxs-lookup"><span data-stu-id="0a18b-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0a18b-p104">אלכימיה תובנות יש רק H1 בודד בחלק העליון או יופר בייצור. H2s אל רינדור כך השתמש **מודגש** או מוסכמות אחרים לשם סימון מקטעים נפרדים.</span><span class="sxs-lookup"><span data-stu-id="0a18b-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0a18b-114">בשלב הבא, למלא את גוף הטקסט באמצעות החומר טיוטה במקטע תובנות של לקוחות של הדף כלל אלכימיה</span><span class="sxs-lookup"><span data-stu-id="0a18b-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0a18b-115">רשימות עם תבליטים הם עדין</span><span class="sxs-lookup"><span data-stu-id="0a18b-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0a18b-116">רשימות ממוספרות מדי</span><span class="sxs-lookup"><span data-stu-id="0a18b-116">Numbered lists too</span></span>
    1. <span data-ttu-id="0a18b-117">**מודגש** *נטוי* הם a-ok</span><span class="sxs-lookup"><span data-stu-id="0a18b-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0a18b-118">קישורים תמיד להיות אחד **"קישורים לאתר" / חיצוני** או **עמוק-קישורים לרכיבי ממשק משתמש**, קישורים פנימיים לא.</span><span class="sxs-lookup"><span data-stu-id="0a18b-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="0a18b-p105">וזו באמת כבר מעט ארוך מדי. שיטת העבודה המומלצת היא כ- 400 תווים---</span><span class="sxs-lookup"><span data-stu-id="0a18b-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0a18b-p106">לאחר התוכן שלך מוכן, למשוך אותו על הענף בשידור חי. לאחר מכן, [פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net) והזן את שם קובץ לתוך שדה כתובת url. ודא תובנה שנסקרו ופורסמו אומר "כן" ולאחר מכן לחץ על עדכון כלל. **(הדבר ייראה תסדר אותה בגירסה החדשה של הפורטל - שחרור בקרוב.)** 
 ![שדה כתובת url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="0a18b-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

