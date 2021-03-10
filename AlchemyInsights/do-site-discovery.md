---
title: בצעו גילוי אתר
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693487"
---
# <a name="do-site-discovery"></a><span data-ttu-id="ad2e2-102">בצעו גילוי אתר</span><span class="sxs-lookup"><span data-stu-id="ad2e2-102">Do site discovery</span></span>

<span data-ttu-id="ad2e2-103">אם הארגון שלך עדיין משתמש ביישומי אינטרנט מדור קודם ובתוכניות לשימוש במצב Internet Explorer (שרוב הלקוחות מבצע), עליך לבצע גילוי אתרים נוסף.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="ad2e2-104">**כבר פרסת גירסה ישנה יותר של Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="ad2e2-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="ad2e2-105">אם כבר הגדרת את רשימת האתרים של הארגון שלך לעבוד עבור הגירסה המורשית של Microsoft Edge, גילוי האתר שלך כמעט מוכן.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="ad2e2-106">הדבר היחיד שייתכן שיהיה עליך לעשות הוא להוסיף אתרים נייטרליים.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="ad2e2-107">אתרים נייטרליים הם בדרך כלל אתרים המספקים כניסה יחידה (SSO).</span><span class="sxs-lookup"><span data-stu-id="ad2e2-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="ad2e2-108">אם אתה עובר לאתר נייטרלי מ-Microsoft Edge, ברצונך להישאר ב-Microsoft Edge כדי לבצע אימות.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="ad2e2-109">אם אתה עובר לאתר נייטרלי במצב Internet Explorer, ברצונך להישאר במצב Internet Explorer כדי לבצע אימות.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="ad2e2-110">זהה את כל ה-SSO או אתרים נייטרליים אחרים שבהם אתה משתמש והוסף אותם לרשימת האתרים הארגוניים שלך.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="ad2e2-111">**Internet Explorer הוא דפדפן ברירת המחדל שלך**</span><span class="sxs-lookup"><span data-stu-id="ad2e2-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="ad2e2-112">אם אתה משתמש רק ב-Internet Explorer כעת, ייתכן שלא תדע אילו אתרים שידרגו לתקני אינטרנט מודרניים ושעדיין דורשים את Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="ad2e2-113">תרצה לחפש ולהוסיף אתרים אלה לרשימת האתרים הארגוניים כדי שתוכל להשתמש במצב Internet Explorer בלבד עבור אתרים אלה.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="ad2e2-114">[גילוי אתר ארגוני](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) מגלה אתרים שעשויים להזדקק למצב Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="ad2e2-115">היא יכולה לאסוף נתונים במחשבים שבהם פועל Windows Internet Explorer 8 באמצעות Internet Explorer 11 ב-Windows 10, Windows 8.1 או Windows 7.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="ad2e2-116">**ניתוח הנתונים**</span><span class="sxs-lookup"><span data-stu-id="ad2e2-116">**Analyze the data**</span></span>

<span data-ttu-id="ad2e2-117">לאחר שאספת את נתוני האתר, מומלץ לבצע את ארבעת השלבים הבאים כדי לנתח את הנתונים:</span><span class="sxs-lookup"><span data-stu-id="ad2e2-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="ad2e2-118">מיין את הנתונים לפי תחום ולאחר מכן לפי כתובת URL.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="ad2e2-119">הגדר את גבולות האפליקציה לקביעת התצורה עבור מצב Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="ad2e2-120">ברצונך לכלול את כל האתרים ופקדי האינטרנט שמגדירים את היישום, אך אין ברצונך לכלול אתרים ופקדים נוספים.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="ad2e2-121">אתרים מסוימים עשויים להיות פשוטים כמו *https://contoso.com/app1* בעוד שאחרים עשויים לדרוש ממך להגדיר אתרים ודפים מרובים.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="ad2e2-122">בדוק את האפליקציה כדי לוודא שהיא אינה פועלת במקור.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="ad2e2-123">אתרים רבים מציעים תוכן מודרני כאשר הם מזהים דפדפן מודרני ומציעים תוכן מדור קודם רק כאשר הם מזהים את Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="ad2e2-124">הוסף את היישום לרשימת האתרים הארגוניים שלך אם הוא נכשל בבדיקה.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="ad2e2-125">כשיטת עבודה מומלצת, קבץ את כל האתרים המרכיבים יישום.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="ad2e2-126">בדרך זו, בעת שדרוג יישום, קל יותר להסיר את האתר כולו ממצב Internet Explorer ולהתחיל להשתמש בדפדפן מודרני עבור יישום זה.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="ad2e2-127">לאחר שתסיים את גילוי האתר וניתחת את הנתונים, אתה מוכן להתחיל להסתכל על אסטרטגיית הערוץ שלך.</span><span class="sxs-lookup"><span data-stu-id="ad2e2-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

