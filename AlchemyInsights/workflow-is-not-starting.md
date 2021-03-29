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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403744"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="07678-102">זרימת העבודה אינה מתחילה</span><span class="sxs-lookup"><span data-stu-id="07678-102">Workflow is not starting</span></span>

- <span data-ttu-id="07678-103">זרימות עבודה של SharePoint 2010 ו- SharePoint 2013 לא מתחילות.</span><span class="sxs-lookup"><span data-stu-id="07678-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="07678-104">אם זרימת העבודה שלך אינה מתחילה, ייתכן שיש בעיית שירות זמנית שבה משתמשים עלולים להיתקל בעיכובים לסירוגין עם התקדמות זרימת העבודה.</span><span class="sxs-lookup"><span data-stu-id="07678-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="07678-105">בדוק את [לוח המחוונים של](https://admin.microsoft.com/AdminPortal/Home/servicehealth) תקינות השירות כדי לראות אם הארגון שלך מושפע.</span><span class="sxs-lookup"><span data-stu-id="07678-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="07678-106">אם עברו יותר מ- 24 שעות מאז הפעם הראשונה שראית בעיה זו, רשום כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="07678-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="07678-107">במקרים רבים, אנחנו כבר עובדים על פתרון.</span><span class="sxs-lookup"><span data-stu-id="07678-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="07678-108">תן לנו לפחות 24 שעות כדי להשלים פתרון.</span><span class="sxs-lookup"><span data-stu-id="07678-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="07678-109">זרימות עבודה של SharePoint 2010 מושהות בתאריך ההתחלה.</span><span class="sxs-lookup"><span data-stu-id="07678-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="07678-110">מצב זה מתרחש אם זרימת העבודה מופעלת באצוות גדולות.</span><span class="sxs-lookup"><span data-stu-id="07678-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="07678-111">(לדוגמה, כאשר כמה פריטים מתווספים בו-זמנית).</span><span class="sxs-lookup"><span data-stu-id="07678-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="07678-112">זרימות עבודה לא מיועדות לפעול בזמן אמת, לכן השהיה היא אופן פעולה של עיצוב לפי עיצוב.</span><span class="sxs-lookup"><span data-stu-id="07678-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="07678-113">אם זרימת העבודה מורכבת שפת סימון אובייקטים מורחבת (XMOL), ההידור יכול להיות איטי.</span><span class="sxs-lookup"><span data-stu-id="07678-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="07678-114">עיין [במאמר](https://support.microsoft.com//kb/3043697) זה.</span><span class="sxs-lookup"><span data-stu-id="07678-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="07678-115">עליך לפשט את זרימת העבודה או לעצב אותה מחדש באמצעות סוג פלטפורמת זרימת העבודה של Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="07678-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="07678-116">אם היסטוריית זרימת העבודה שלך גדלה, ייתכן שתרצה לנקות את הפריטים או ליצור רשימת היסטוריה חדשה.</span><span class="sxs-lookup"><span data-stu-id="07678-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="07678-117">מידע נוסף : [ניקוי היסטוריית זרימת עבודה](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="07678-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="07678-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="07678-118">Related topics</span></span>
<span data-ttu-id="07678-119">רוצה לנסות את Microsoft Flow ב- SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="07678-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="07678-120">יצירת זרימה</span><span class="sxs-lookup"><span data-stu-id="07678-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="07678-121">SharePoint ו- Flow</span><span class="sxs-lookup"><span data-stu-id="07678-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
