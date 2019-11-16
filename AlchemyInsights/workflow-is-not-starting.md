---
title: זרימת עבודה אינה מתחילה
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738090"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="afb34-102">זרימת עבודה אינה מתחילה</span><span class="sxs-lookup"><span data-stu-id="afb34-102">Workflow is not starting</span></span>

- <span data-ttu-id="afb34-103">זרימות עבודה של SharePoint 2010 ו-SharePoint 2013 אינן מתחילות.</span><span class="sxs-lookup"><span data-stu-id="afb34-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="afb34-104">אם זרימת העבודה שלך אינה מתחילה, ייתכן שקיימת בעיית שירות זמנית שבה משתמשים עלולים להיתקל בעיכובים לסירוגין עם התקדמות זרימת העבודה.</span><span class="sxs-lookup"><span data-stu-id="afb34-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="afb34-105">בדוק את [לוח הבקרה של תקינות השירות](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק אם הארגון שלך מושפע.</span><span class="sxs-lookup"><span data-stu-id="afb34-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="afb34-106">אם חלפו יותר מ -24 שעות מאז הפעם הראשונה שראית את הנושא הזה, אנא התחבר כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="afb34-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="afb34-107">במקרים רבים, אנחנו כבר עובדים על פתרון.</span><span class="sxs-lookup"><span data-stu-id="afb34-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="afb34-108">בבקשה תן לנו לפחות 24. שעות כדי להשלים פיתרון</span><span class="sxs-lookup"><span data-stu-id="afb34-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="afb34-109">זרימות עבודה של SharePoint 2010 איחרו בהתחלה.</span><span class="sxs-lookup"><span data-stu-id="afb34-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="afb34-110">מצב זה מתרחש אם זרימת העבודה מופעלת באצוות גדולות.</span><span class="sxs-lookup"><span data-stu-id="afb34-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="afb34-111">(לדוגמה, כאשר מספר פריטים נוספים בבת אחת).</span><span class="sxs-lookup"><span data-stu-id="afb34-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="afb34-112">זרימות עבודה אינן מתוכננות לפעול בזמן אמת, כך שהשהיה היא התנהגות לפי עיצוב.</span><span class="sxs-lookup"><span data-stu-id="afb34-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="afb34-113">אם זרימת העבודה היא שפת סימון אובייקט מורחבת מורכבת (XMOL), ההידור יכול להיות איטי.</span><span class="sxs-lookup"><span data-stu-id="afb34-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="afb34-114">בדוק [את המאמר](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="afb34-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="afb34-115">עליך לפשט את זרימת העבודה או לעצב אותה מחדש באמצעות סוג פלטפורמת זרימת העבודה של Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="afb34-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="afb34-116">אם היסטוריית זרימת העבודה שלך גדלה בגדול, ייתכן שתרצה למחוק את הפריטים או ליצור רשימת היסטוריה חדשה.</span><span class="sxs-lookup"><span data-stu-id="afb34-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="afb34-117">מידע נוסף: [נקה היסטוריית זרימת עבודה](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="afb34-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="afb34-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="afb34-118">Related topics</span></span>
<span data-ttu-id="afb34-119">רוצה לנסות את Microsoft Flow ב-SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="afb34-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="afb34-120">צור זרימה</span><span class="sxs-lookup"><span data-stu-id="afb34-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="afb34-121">SharePoint וזרימה</span><span class="sxs-lookup"><span data-stu-id="afb34-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


