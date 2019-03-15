---
title: 'זהה filename הוא הטוב ביותר [כלל #-תיאור]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634505"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="679b5-102">נדרש אלכימיה כותרת H1, H2 של אינם פועלים.</span><span class="sxs-lookup"><span data-stu-id="679b5-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="679b5-103">ושיטות עבודה מומלצות הנחיות לעריכת אלכימיה:</span><span class="sxs-lookup"><span data-stu-id="679b5-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="679b5-104">**לא לקנן תובנות אלכימיה בתיקיות**- פעולה זו תנתק את מבנה ה-url.</span><span class="sxs-lookup"><span data-stu-id="679b5-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="679b5-105">אנו מביט לתוך תיקון זה.</span><span class="sxs-lookup"><span data-stu-id="679b5-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="679b5-106">הקבצים בתיקיה **AlchemyInsights** צריך להיות מזהה כלל ושם כלל מתוך [פורטל השותפים אלכימיה של](https://alchemyportal.azurewebsites.net) שם הקובץ.</span><span class="sxs-lookup"><span data-stu-id="679b5-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="679b5-107">ex.</span><span class="sxs-lookup"><span data-stu-id="679b5-107">ex.</span></span> <span data-ttu-id="679b5-108">***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="679b5-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="679b5-109">השתמש את המטה-נתונים בחלק העליון של קובץ זה כתבנית שלך.</span><span class="sxs-lookup"><span data-stu-id="679b5-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="679b5-110">דבר נוסף נדרש.</span><span class="sxs-lookup"><span data-stu-id="679b5-110">Nothing else is required.</span></span>
1. <span data-ttu-id="679b5-111">[פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net), נווט למטה למקטע **הכותרת תובנות לקוח:** ושימוש המצביעים בתור התחלה עבור כותרת H1 שלך לקבלת תובנות.</span><span class="sxs-lookup"><span data-stu-id="679b5-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="679b5-112">אלכימיה תובנות יש רק H1 בודד בחלק העליון או יופר בייצור.</span><span class="sxs-lookup"><span data-stu-id="679b5-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="679b5-113">H2s אל רינדור כך השתמש **מודגש** או מוסכמות אחרים לשם סימון מקטעים נפרדים.</span><span class="sxs-lookup"><span data-stu-id="679b5-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="679b5-114">בשלב הבא, למלא את גוף הטקסט באמצעות החומר טיוטה במקטע תובנות של לקוחות של הדף כלל אלכימיה</span><span class="sxs-lookup"><span data-stu-id="679b5-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="679b5-115">רשימות עם תבליטים הם עדין</span><span class="sxs-lookup"><span data-stu-id="679b5-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="679b5-116">רשימות ממוספרות מדי</span><span class="sxs-lookup"><span data-stu-id="679b5-116">Numbered lists too</span></span>
    1. <span data-ttu-id="679b5-117">**מודגש** *נטוי* הם a-ok</span><span class="sxs-lookup"><span data-stu-id="679b5-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="679b5-118">קישורים תמיד להיות אחד **"קישורים לאתר" / חיצוני** או **עמוק-קישורים לרכיבי ממשק משתמש**, קישורים פנימיים לא.</span><span class="sxs-lookup"><span data-stu-id="679b5-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="679b5-119">וזו באמת כבר מעט ארוך מדי.</span><span class="sxs-lookup"><span data-stu-id="679b5-119">And this is really already a bit too long.</span></span> <span data-ttu-id="679b5-120">שיטת העבודה המומלצת היא כ- 400 תווים---</span><span class="sxs-lookup"><span data-stu-id="679b5-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="679b5-121">לאחר התוכן שלך מוכן, למשוך אותו על הענף בשידור חי.</span><span class="sxs-lookup"><span data-stu-id="679b5-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="679b5-122">לאחר מכן, [פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net) והזן את שם קובץ לתוך שדה כתובת url.</span><span class="sxs-lookup"><span data-stu-id="679b5-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="679b5-123">ודא תובנה שנסקרו ופורסמו אומר "כן" ולאחר מכן לחץ על עדכון כלל.</span><span class="sxs-lookup"><span data-stu-id="679b5-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="679b5-124">**(הדבר ייראה תסדר אותה בגירסה החדשה של הפורטל - שחרור בקרוב.)** 
 ![שדה כתובת url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="679b5-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

