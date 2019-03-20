---
title: בדיוק כמו שם הקובץ הוא הטוב ביותר
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683850"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="988ff-102">נדרש אלכימיה כותרת H1, H2 של אינם פועלים.</span><span class="sxs-lookup"><span data-stu-id="988ff-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="988ff-103">ושיטות עבודה מומלצות הנחיות לעריכת אלכימיה:</span><span class="sxs-lookup"><span data-stu-id="988ff-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="988ff-104">**לא לקנן תובנות אלכימיה בתיקיות**- פעולה זו תנתק את מבנה ה-url.</span><span class="sxs-lookup"><span data-stu-id="988ff-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="988ff-105">אנו מביט לתוך תיקון זה.</span><span class="sxs-lookup"><span data-stu-id="988ff-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="988ff-106">הקבצים בתיקיה **AlchemyInsights** יש שמות קבצים באותיות קטנות עם מקפים רווחים לדוגמה.</span><span class="sxs-lookup"><span data-stu-id="988ff-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="988ff-107">***how-to-אפשר-תביעה משפטית-חסימה***.</span><span class="sxs-lookup"><span data-stu-id="988ff-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="988ff-108">כלול את מזהה מזהה כלל או דלי מתוך [פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net) בשדה ms.custom.</span><span class="sxs-lookup"><span data-stu-id="988ff-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="988ff-109">ex.</span><span class="sxs-lookup"><span data-stu-id="988ff-109">ex.</span></span> <span data-ttu-id="988ff-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="988ff-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="988ff-111">שימוש יתר של המטה-נתונים בחלק העליון של קובץ זה כתבנית שלך.</span><span class="sxs-lookup"><span data-stu-id="988ff-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="988ff-112">[פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net), נווט למטה למקטע **הכותרת תובנות לקוח:** ושימוש המצביעים בתור התחלה עבור כותרת H1 שלך לקבלת תובנות.</span><span class="sxs-lookup"><span data-stu-id="988ff-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="988ff-113">אלכימיה תובנות יש רק H1 בודד בחלק העליון או יופר בייצור.</span><span class="sxs-lookup"><span data-stu-id="988ff-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="988ff-114">H2s אל רינדור כך השתמש **מודגש** או מוסכמות אחרים לשם סימון מקטעים נפרדים.</span><span class="sxs-lookup"><span data-stu-id="988ff-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="988ff-115">בשלב הבא, למלא את גוף הטקסט באמצעות החומר טיוטה במקטע תובנות של לקוחות של הדף כלל אלכימיה</span><span class="sxs-lookup"><span data-stu-id="988ff-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="988ff-116">רשימות עם תבליטים הם עדין</span><span class="sxs-lookup"><span data-stu-id="988ff-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="988ff-117">רשימות ממוספרות מדי</span><span class="sxs-lookup"><span data-stu-id="988ff-117">Numbered lists too</span></span>
    1. <span data-ttu-id="988ff-118">**מודגש** *נטוי* הם a-ok</span><span class="sxs-lookup"><span data-stu-id="988ff-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="988ff-119">קישורים תמיד להיות אחד **"קישורים לאתר" / חיצוני** או **עמוק-קישורים לרכיבי ממשק משתמש**, קישורים פנימיים לא.</span><span class="sxs-lookup"><span data-stu-id="988ff-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="988ff-120">תמונות לא נתמכים באופן רשמי לעת עתה, אך הוא מופיע על מפת דרכים.</span><span class="sxs-lookup"><span data-stu-id="988ff-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="988ff-121">וזו באמת כבר מעט ארוך מדי.</span><span class="sxs-lookup"><span data-stu-id="988ff-121">And this is really already a bit too long.</span></span> <span data-ttu-id="988ff-122">שיטת העבודה המומלצת היא כ- 400 תווים---</span><span class="sxs-lookup"><span data-stu-id="988ff-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="988ff-123">לאחר התוכן שלך מוכן, למשוך אותו על הענף בשידור חי.</span><span class="sxs-lookup"><span data-stu-id="988ff-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="988ff-124">לאחר מכן, [פורטל השותפים אלכימיה](https://alchemyportal.azurewebsites.net) והזן את שם קובץ לתוך שדה כתובת url.</span><span class="sxs-lookup"><span data-stu-id="988ff-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="988ff-125">M</span><span class="sxs-lookup"><span data-stu-id="988ff-125">M</span></span>