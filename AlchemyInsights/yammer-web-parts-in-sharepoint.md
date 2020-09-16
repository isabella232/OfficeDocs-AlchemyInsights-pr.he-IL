---
title: רכיבי web part של קטרת ב-SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664351"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="e3585-102">רכיבי web part של קטרת ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3585-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="e3585-103">שיחות קטרת ו-קטרת web parts משפרים את שיתוף הפעולה בדפי SharePoint מודרניים וקלאסיים.</span><span class="sxs-lookup"><span data-stu-id="e3585-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="e3585-104">לקבלת מידע נוסף, ראה [שיחות קטרת](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  [ונקודות](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)מרכזיות של קטרת.</span><span class="sxs-lookup"><span data-stu-id="e3585-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="e3585-105">ה-web part המודרני של שיחות קטרת מתעדכן לחוויית קטרת החדשה והוא זמין עבור דיירי שחרור ממוקד.</span><span class="sxs-lookup"><span data-stu-id="e3585-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="e3585-106">השקת GA הופעלה.</span><span class="sxs-lookup"><span data-stu-id="e3585-106">GA rollout has started.</span></span> <span data-ttu-id="e3585-107">תכונות חדשות כוללות את היכולת להתחיל שיחה עם כל פרסום (שאלות, סקרים, השבחה) ולסמן את התשובות הטובות ביותר ישירות מ-SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e3585-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="e3585-108">לקבלת מידע נוסף, ראה [מונחים חדשים של קטרת customers ושאלות נפוצות](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="e3585-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="e3585-109">כדי להבין איזה web part וקביעת תצורה מתאימה לך, ראה שימוש ב-web part של [קטרת ב-SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="e3585-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="e3585-110">**שימוש ב-web parts עם SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="e3585-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="e3585-111">ניתן להשתמש ברכיבי Web part בדפים מודרניים וקלאסיים בתוך סביבות מקומיות.</span><span class="sxs-lookup"><span data-stu-id="e3585-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="e3585-112">לקבלת מידע נוסף אודות דפים מודרניים, ראה [הוספת הזנת קטרת לעמוד מודרני ב-SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="e3585-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="e3585-113">לקבלת מידע נוסף אודות עמודים קלאסיים, ראה [הוספת הזנת קטרת לעמוד קלאסי בשרתי SharePoint 2013, 2016 ו-2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="e3585-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="e3585-114">**קטרת Embed**</span><span class="sxs-lookup"><span data-stu-id="e3585-114">**Yammer Embed**</span></span>  

<span data-ttu-id="e3585-115">השתמש בכלי ' קביעת תצורה של הטבעה ' כדי לבדוק את השימוש בהטבעה.</span><span class="sxs-lookup"><span data-stu-id="e3585-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="e3585-116">עדכון עתידי להטבעה יהפוך את החוויה החדשה של קטרת לזמינה.</span><span class="sxs-lookup"><span data-stu-id="e3585-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="e3585-117">לקבלת מידע נוסף, עיין [בכלי קביעת התצורה של קטרת Embed](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="e3585-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="e3585-118">כדי להבין טוב יותר את רכיב ההטבעה של קטרת, ראה [הטבעת הזנה](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="e3585-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="e3585-119">**בעיות ידועות ומגבלות**</span><span class="sxs-lookup"><span data-stu-id="e3585-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="e3585-120">מזהי קבוצה אינם זמינים בכתובות Url חדשות של קטרת, שהשתנו.</span><span class="sxs-lookup"><span data-stu-id="e3585-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="e3585-121">עבור בחזרה למצב קלאסי כדי לקבל מזהי קבוצה או מזהים אחרים מכתובות Url.</span><span class="sxs-lookup"><span data-stu-id="e3585-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="e3585-122">תחומים מותאמים אישית (יוהרה) אינם נתמכים.</span><span class="sxs-lookup"><span data-stu-id="e3585-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="e3585-123">קטרת Embed אינו ממוטב עבור mobile.</span><span class="sxs-lookup"><span data-stu-id="e3585-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="e3585-124">השתמש בדפים מודרניים עם ה-web part של שיחות קטרת לקבלת החוויה הטובה ביותר.</span><span class="sxs-lookup"><span data-stu-id="e3585-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="e3585-125">ערכות נושא מותאמות אישית יכולות להשפיע על המראה והשימושיות של ה-web part של שיחות קטרת.</span><span class="sxs-lookup"><span data-stu-id="e3585-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="e3585-126">פתח מקרה תמיכה כדי לדווח על בעיות.</span><span class="sxs-lookup"><span data-stu-id="e3585-126">Open a support case to report issues.</span></span>