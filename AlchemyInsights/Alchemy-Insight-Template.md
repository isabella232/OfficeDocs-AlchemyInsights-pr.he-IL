---
title: הצורה הטובה ביותר לשמות השמות
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664135"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0c67c-102">"נדרשת כותרת האלכימיה H1, H2's לא פועל".</span><span class="sxs-lookup"><span data-stu-id="0c67c-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="0c67c-103">שיטות עבודה מומלצות וקווים מנחים לעריכה באלכימיה:</span><span class="sxs-lookup"><span data-stu-id="0c67c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0c67c-104">**אל תקנן תובנות אלכימיה בתיקיות**-פעולה זו תשבור את מבנה כתובת ה-url.</span><span class="sxs-lookup"><span data-stu-id="0c67c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="0c67c-105">אנחנו מעוניינים לתקן זאת.</span><span class="sxs-lookup"><span data-stu-id="0c67c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="0c67c-106">קבצים בתיקיית **AlchemyInsights** אמורים לכלול שמות קבצים באותיות קטנות עם מקפים עבור רווחים לשעבר.</span><span class="sxs-lookup"><span data-stu-id="0c67c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="0c67c-107">***כיצד להפוך לזמינים-ליטיגציה-המתנה***.</span><span class="sxs-lookup"><span data-stu-id="0c67c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="0c67c-108">כלול את מזהה הכלל או את מזהה הדלי [מפורטל השותפים לאלכימיה](https://alchemyportal.azurewebsites.net) בשדה ms. custom.</span><span class="sxs-lookup"><span data-stu-id="0c67c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="0c67c-109">דוגמה.</span><span class="sxs-lookup"><span data-stu-id="0c67c-109">ex.</span></span> <span data-ttu-id="0c67c-110">***ms. custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="0c67c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="0c67c-111">השתמש בשאר המטה-נתונים בחלק העליון של קובץ זה כתבנית.</span><span class="sxs-lookup"><span data-stu-id="0c67c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="0c67c-112">בפורטל [השותפים לאלכימיה](https://alchemyportal.azurewebsites.net), נווט מטה אל **כותרת התובנה של לקוח** המקטע: והשתמש בה כנקודת התחלה עבור כותרת H1 עבור התובנה.</span><span class="sxs-lookup"><span data-stu-id="0c67c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0c67c-113">תובנות של אלכימיה חייבות לכלול רק H1 אחד בחלק העליון, או שהם ישברו בייצור.</span><span class="sxs-lookup"><span data-stu-id="0c67c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="0c67c-114">H2s אינם מוצגים כך שעליך להשתמש במוסכמות **מודגשות** או אחרות כדי לסמן מקטעים נפרדים.</span><span class="sxs-lookup"><span data-stu-id="0c67c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0c67c-115">לאחר מכן, מלא את הטקסט בגוף באמצעות חומר הטיוטה במקטע ' תובנות לקוח ' בדף ' כלל אלכימיה '</span><span class="sxs-lookup"><span data-stu-id="0c67c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0c67c-116">רשימות עם תבליטים בסדר</span><span class="sxs-lookup"><span data-stu-id="0c67c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0c67c-117">רשימות ממוספרות מדי</span><span class="sxs-lookup"><span data-stu-id="0c67c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="0c67c-118">**Bold** מודגש *ונטוי* הם a-ok</span><span class="sxs-lookup"><span data-stu-id="0c67c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0c67c-119">קישורים אמורים להיות תמיד **' קישורים לאינטרנט '/external ' או '** **קישורים עמוקים ' לרכיבי ממשק משתמש**, ולא לקישורים פנימיים.</span><span class="sxs-lookup"><span data-stu-id="0c67c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="0c67c-120">התמונות אינן נתמכות באופן רשמי בשלב זה, אך היא נמצאת במפת הדרכים.</span><span class="sxs-lookup"><span data-stu-id="0c67c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="0c67c-121">וזה באמת כבר זמן רב מדי.</span><span class="sxs-lookup"><span data-stu-id="0c67c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="0c67c-122">העבודה הטובה ביותר היא לגבי 400 תווים---------------------------------</span><span class="sxs-lookup"><span data-stu-id="0c67c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0c67c-123">לאחר שהתוכן שלך מוכן, משוך אותו לענף החי.</span><span class="sxs-lookup"><span data-stu-id="0c67c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="0c67c-124">לאחר מכן, עבור אל [פורטל השותפים לאלכימיה](https://alchemyportal.azurewebsites.net) והזן את שם הקובץ בשדה כתובת ה-url.</span><span class="sxs-lookup"><span data-stu-id="0c67c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 