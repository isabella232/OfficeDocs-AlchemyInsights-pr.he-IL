---
title: Web parts של יממר ב-SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198063"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="652d4-102">Web parts של יממר ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="652d4-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="652d4-103">שיחות יממר ו-Yammer מדגיש חלקי אינטרנט לשפר את שיתוף הפעולה על דפי SharePoint מודרני וקלאסי.</span><span class="sxs-lookup"><span data-stu-id="652d4-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="652d4-104">לקבלת מידע נוסף, ראה [שיחות מיאמר](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) [והדגמר](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span><span class="sxs-lookup"><span data-stu-id="652d4-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="652d4-105">ה-web part המודרני של שיחות Yammer מתעדכן לחווית Yammer החדשה והוא זמין עבור הדיירים שחרור ממוקד.</span><span class="sxs-lookup"><span data-stu-id="652d4-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="652d4-106">התחלת השקת GA.</span><span class="sxs-lookup"><span data-stu-id="652d4-106">GA rollout has started.</span></span> <span data-ttu-id="652d4-107">תכונות חדשות כוללות את היכולת להתחיל שיחה עם כל הודעה (שאלות, סקרים, שבח) ולסמן את התשובות הטובות ביותר ישירות מ-SharePoint.</span><span class="sxs-lookup"><span data-stu-id="652d4-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="652d4-108">לקבלת מידע נוסף, ראה [מונחי לקוח חדשים ושאלות נפוצות](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="652d4-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="652d4-109">כדי להבין איזה web part וקביעת תצורה מימין עבורך, ראה [שימוש ב-web part של Yammer ב-SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="652d4-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="652d4-110">**שימוש בחלקי אינטרנט באמצעות SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="652d4-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="652d4-111">ניתן להשתמש בחלקי אינטרנט בעמודים מודרניים וקלאסיים בתוך סביבות מקומיות.</span><span class="sxs-lookup"><span data-stu-id="652d4-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="652d4-112">לקבלת מידע נוסף על עמודים מודרניים, ראה [הוספת הזנת Yammer לדף מודרני ב-SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="652d4-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="652d4-113">לקבלת מידע נוסף אודות דפים קלאסיים, ראה [הוספת הזנה של Yammer לדף קלאסי בשרתי SharePoint 2013, 2016 ו-2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="652d4-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="652d4-114">**הטבעת מימר**</span><span class="sxs-lookup"><span data-stu-id="652d4-114">**Yammer Embed**</span></span>  

<span data-ttu-id="652d4-115">השתמש בכלי קביעת תצורת הטבעה כדי לבדוק את השימוש בהטבעה.</span><span class="sxs-lookup"><span data-stu-id="652d4-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="652d4-116">עדכון עתידי להטבעה יאפשר לחווית יממר החדשה.</span><span class="sxs-lookup"><span data-stu-id="652d4-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="652d4-117">לקבלת מידע נוסף, עיין [בכלי ' קביעת תצורת הטבעה של יממר](https://aka.ms/YammerEmbedConfigureTool)'.</span><span class="sxs-lookup"><span data-stu-id="652d4-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="652d4-118">כדי להבין טוב יותר את רכיב הטבעה של ימר, ראה [הטבעת הזנה](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="652d4-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="652d4-119">**בעיות והגבלות ידועות**</span><span class="sxs-lookup"><span data-stu-id="652d4-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="652d4-120">מזהי קבוצה אינם זמינים מכתובות Url חדשות של Yammer, שהשתנו.</span><span class="sxs-lookup"><span data-stu-id="652d4-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="652d4-121">עבור חזרה למצב הקלאסי כדי לקבל מזהי קבוצה או מזהים אחרים מכתובות Url.</span><span class="sxs-lookup"><span data-stu-id="652d4-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="652d4-122">אין תמיכה בתחומים מותאמים אישית (יהירות).</span><span class="sxs-lookup"><span data-stu-id="652d4-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="652d4-123">הטמע yammer אינו ממוטב עבור ניידים.</span><span class="sxs-lookup"><span data-stu-id="652d4-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="652d4-124">השתמש בדפים מודרניים עם ה-web part ' שיחות יממר ' לחוויה הטובה ביותר.</span><span class="sxs-lookup"><span data-stu-id="652d4-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="652d4-125">ערכות נושא מותאמות אישית יכולות להשפיע על המראה והשימושיות של ה-web part של שיחות Yammer.</span><span class="sxs-lookup"><span data-stu-id="652d4-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="652d4-126">פתח אירוע תמיכה כדי לדווח על בעיות.</span><span class="sxs-lookup"><span data-stu-id="652d4-126">Open a support case to report issues.</span></span>