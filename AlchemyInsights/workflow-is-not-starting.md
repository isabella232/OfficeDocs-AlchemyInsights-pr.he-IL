---
title: זרימת העבודה לא מופעל
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270781"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="49aa5-102">זרימת העבודה לא מופעל</span><span class="sxs-lookup"><span data-stu-id="49aa5-102">Workflow is not starting</span></span>

- <span data-ttu-id="49aa5-103">זרימות עבודה של SharePoint 2010 ו- SharePoint 2013 אתה לא מתחיל.</span><span class="sxs-lookup"><span data-stu-id="49aa5-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="49aa5-104">אם זרימת העבודה שלך לא מופעל, ייתכן שקיימת בעיית שירות זמני שבו משתמשים עלולים להיתקל עיכובים לסירוגין עם התקדמות זרימת העבודה.</span><span class="sxs-lookup"><span data-stu-id="49aa5-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="49aa5-105">בדוק את [לוח המחוונים של תקינות השירות](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לראות אם הארגון שלך מושפע.</span><span class="sxs-lookup"><span data-stu-id="49aa5-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="49aa5-106">אם יותר מ- 24 שעות חלפו מאז שראית תחילה את הבעיה, היכנס כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="49aa5-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="49aa5-107">במקרים רבים, אנו אתה כבר עובד על פתרון.</span><span class="sxs-lookup"><span data-stu-id="49aa5-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="49aa5-108">נא תן לנו לפחות 24 שעות להשלמת פתרון.</span><span class="sxs-lookup"><span data-stu-id="49aa5-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="49aa5-109">זרימות עבודה של SharePoint 2010 איחור בהתחלת.</span><span class="sxs-lookup"><span data-stu-id="49aa5-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="49aa5-110">מצב זה מתרחש אם זרימת העבודה מופעלת בקבוצות גדולות.</span><span class="sxs-lookup"><span data-stu-id="49aa5-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="49aa5-111">(לדוגמה, כאשר מספר פריטים נוספים בבת אחת).</span><span class="sxs-lookup"><span data-stu-id="49aa5-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="49aa5-112">זרימות עבודה אינה מיועדת לפעול בזמן אמת, כך עיכוב היא על-ידי עיצוב התנהגות.</span><span class="sxs-lookup"><span data-stu-id="49aa5-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="49aa5-113">אם זרימת העבודה הוא מורכב להרחבה האובייקט סימון השפה (XMOL), יכול להיות איטי הידור.</span><span class="sxs-lookup"><span data-stu-id="49aa5-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="49aa5-114">בדוק מאמר [זה](https://support.microsoft.com/en-us/kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="49aa5-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="49aa5-115">עליך לפשט את זרימת העבודה או לעצב אותו באמצעות סוג פלטפורמה של Microsoft SharePoint 2013 זרימת מחדש.</span><span class="sxs-lookup"><span data-stu-id="49aa5-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="49aa5-116">אם היסטוריית זרימת העבודה שלך גדלה גדול יותר, ייתכן שתרצה למחוק לצמיתות את הפריטים או ליצור רשימת היסטוריה חדשה.</span><span class="sxs-lookup"><span data-stu-id="49aa5-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="49aa5-117">מידע נוסף: [ניקוי היסטוריית זרימת עבודה](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="49aa5-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="49aa5-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="49aa5-118">Related topics</span></span>
<span data-ttu-id="49aa5-119">מעוניין לנסות זרימה Microsoft ב- SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="49aa5-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="49aa5-120">צור זרימה</span><span class="sxs-lookup"><span data-stu-id="49aa5-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="49aa5-121">SharePoint וזרימה</span><span class="sxs-lookup"><span data-stu-id="49aa5-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


