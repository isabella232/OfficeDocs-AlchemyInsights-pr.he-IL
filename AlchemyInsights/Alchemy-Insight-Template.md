---
title: זהה לשם הקובץ הטוב ביותר
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750971"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="e83d5-102">"כותרת האלכימיה הנדרשת H1, H2's לא עובד."</span><span class="sxs-lookup"><span data-stu-id="e83d5-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="e83d5-103">שיטות עבודה מומלצות והנחיות לעריכת האלכימיה:</span><span class="sxs-lookup"><span data-stu-id="e83d5-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="e83d5-104">אל **תקנן את האלכימיה תובנות בתיקיות**-זה ישבור את מבנה כתובת האתר.</span><span class="sxs-lookup"><span data-stu-id="e83d5-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="e83d5-105">אנחנו בודקים. את התיקון הזה</span><span class="sxs-lookup"><span data-stu-id="e83d5-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="e83d5-106">קבצים בתיקיה **Alchemyinsights** אמורים להיות בעלי שמות קבצים באותיות קטנות עם מקפים עבור רווחים לשעבר.</span><span class="sxs-lookup"><span data-stu-id="e83d5-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="e83d5-107">***כיצד לאפשר-ליטיגציה-חסימה***.</span><span class="sxs-lookup"><span data-stu-id="e83d5-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="e83d5-108">כלול את מזהה הכלל או את מזהה הדלי מתוך [הפורטל השותף של האלכימיה](https://alchemyportal.azurewebsites.net) בשדה המותאם אישית של ms.</span><span class="sxs-lookup"><span data-stu-id="e83d5-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="e83d5-109">לשעבר.</span><span class="sxs-lookup"><span data-stu-id="e83d5-109">ex.</span></span> <span data-ttu-id="e83d5-110">***מותאם אישית: 100021***</span><span class="sxs-lookup"><span data-stu-id="e83d5-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="e83d5-111">השתמש בשאר המטא-נתונים בחלק העליון של קובץ זה כתבנית.</span><span class="sxs-lookup"><span data-stu-id="e83d5-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="e83d5-112">בפורטל [השותפים של האלכימיה](https://alchemyportal.azurewebsites.net), נווט למטה אל **כותרת התובנה של הלקוח:** והשתמש בו כנקודת התחלה עבור כותרת ה-H1 שלך לתובנה.</span><span class="sxs-lookup"><span data-stu-id="e83d5-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="e83d5-113">אלכימיה התובנות צריכות להיות רק H1 אחד בראש או שהם ישברו בהפקה.</span><span class="sxs-lookup"><span data-stu-id="e83d5-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="e83d5-114">H2s לא משתמשים במוסכמות **מודגשות** או אחרות כדי לציין סעיפים נפרדים.</span><span class="sxs-lookup"><span data-stu-id="e83d5-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="e83d5-115">לאחר מכן, מלא את גוף הטקסט באמצעות החומר הטיוטה בסעיף ' תובנות לקוחות ' בעמוד ' כלל האלכימיה '</span><span class="sxs-lookup"><span data-stu-id="e83d5-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="e83d5-116">רשימות עם תבליטים הן בסדר</span><span class="sxs-lookup"><span data-stu-id="e83d5-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="e83d5-117">גם רשימות ממוספרות</span><span class="sxs-lookup"><span data-stu-id="e83d5-117">Numbered lists too</span></span>
    1. <span data-ttu-id="e83d5-118">**Bold** מודגש *ונטוי* הם בסדר</span><span class="sxs-lookup"><span data-stu-id="e83d5-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="e83d5-119">על הקישורים להיות תמיד **' קישורים לאינטרנט '/' חיצוני ' או '** קישורים עמוקים ' **לרכיבי UI**, לא קישורים פנימיים.</span><span class="sxs-lookup"><span data-stu-id="e83d5-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="e83d5-120">התמונות אינן נתמכות באופן רשמי בשלב זה, אך היא נמצאת במפת הדרכים.</span><span class="sxs-lookup"><span data-stu-id="e83d5-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="e83d5-121">. וזה באמת כבר יותר מדי זמן</span><span class="sxs-lookup"><span data-stu-id="e83d5-121">And this is really already a bit too long.</span></span> <span data-ttu-id="e83d5-122">האימון הטוב ביותר הוא כ-400 תווים---------------------------------</span><span class="sxs-lookup"><span data-stu-id="e83d5-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="e83d5-123">לאחר שהתוכן שלך מוכן, משוך אותו לענף החי.</span><span class="sxs-lookup"><span data-stu-id="e83d5-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="e83d5-124">לאחר מכן, עבור אל [הפורטל השותף של אלכימיה](https://alchemyportal.azurewebsites.net) והזן את שם הקובץ בשדה url.</span><span class="sxs-lookup"><span data-stu-id="e83d5-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 