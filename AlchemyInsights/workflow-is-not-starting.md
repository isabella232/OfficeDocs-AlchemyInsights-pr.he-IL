---
title: זרימת העבודה אינה מתחילה
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794768"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="a578a-102">זרימת העבודה אינה מתחילה</span><span class="sxs-lookup"><span data-stu-id="a578a-102">Workflow is not starting</span></span>

- <span data-ttu-id="a578a-103">זרימות עבודה של SharePoint 2010 ו-SharePoint 2013 אינן מתחילות.</span><span class="sxs-lookup"><span data-stu-id="a578a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="a578a-104">אם זרימת העבודה אינה מופעלת, ייתכן שקיימת בעיה זמנית בשירות שבו משתמשים עשויים להיתקל בעיכובים רציפים בהתקדמות זרימת העבודה.</span><span class="sxs-lookup"><span data-stu-id="a578a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="a578a-105">בדוק את [לוח המחוונים של תקינות השירות](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק אם הארגון שלך מושפע.</span><span class="sxs-lookup"><span data-stu-id="a578a-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="a578a-106">אם חלפו יותר מ-24 שעות מאז שראית בעיה זו לראשונה, רשום כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="a578a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a578a-107">במקרים רבים, אנו כבר עובדים על פתרון.</span><span class="sxs-lookup"><span data-stu-id="a578a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a578a-108">אנא תן לנו לפחות 24 שעות כדי להשלים פתרון.</span><span class="sxs-lookup"><span data-stu-id="a578a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="a578a-109">זרימות עבודה של SharePoint 2010 מעוכבות בעת ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="a578a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="a578a-110">מצב זה מתרחש אם זרימת העבודה מופעלת באצוות גדולים.</span><span class="sxs-lookup"><span data-stu-id="a578a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="a578a-111">(לדוגמה, כאשר מספר פריטים נוספים בבת אחת).</span><span class="sxs-lookup"><span data-stu-id="a578a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="a578a-112">זרימות עבודה אינן מיועדות לפעול בזמן אמת, ולכן השהיה היא לפי עיצוב.</span><span class="sxs-lookup"><span data-stu-id="a578a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="a578a-113">אם זרימת העבודה היא שפת סימון אובייקט מורכבת הניתנת להרחבה (XMOL), הידור עשוי להיות איטי.</span><span class="sxs-lookup"><span data-stu-id="a578a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="a578a-114">סמן מאמר [זה](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="a578a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="a578a-115">עליך לפשט את זרימת העבודה או לעצב אותה מחדש באמצעות סוג פלטפורמת זרימת העבודה של Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="a578a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="a578a-116">אם היסטוריית זרימת העבודה שלך גדלה, ייתכן שתרצה למחוק את הפריטים או ליצור רשימת היסטוריה חדשה.</span><span class="sxs-lookup"><span data-stu-id="a578a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="a578a-117">מידע נוסף: [ניקוי היסטוריית זרימת עבודה](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="a578a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="a578a-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="a578a-118">Related topics</span></span>
<span data-ttu-id="a578a-119">מעוניין לנסות את Microsoft Flow ב-SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a578a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a578a-120">יצירת זרימה</span><span class="sxs-lookup"><span data-stu-id="a578a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a578a-121">SharePoint ו-Flow</span><span class="sxs-lookup"><span data-stu-id="a578a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


