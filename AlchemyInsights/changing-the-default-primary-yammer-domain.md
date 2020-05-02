---
title: שינוי תחום ברירת המחדל של Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991196"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="6bf74-102">שינוי תחום ברירת המחדל/הראשי של Yammer</span><span class="sxs-lookup"><span data-stu-id="6bf74-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="6bf74-103">כתובת ה- URL של Yammer מכילה את שם התחום הראשי הנוכחי עבור רשת Yammer שלך.</span><span class="sxs-lookup"><span data-stu-id="6bf74-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="6bf74-104">ייתכן ששם תחום זה לא יתאים לשם התחום הראשי שנקבע ב-Office 365 או ב- Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6bf74-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="6bf74-105">קיימים הבדלים בהתנהגות בהתבסס על מספר התחומים המותאמים אישית שנוספו לדייר, ואם Yammer מוגדר תחת תצורה נתמכת (דייר 1: רשת 1, או אחד על אחד).</span><span class="sxs-lookup"><span data-stu-id="6bf74-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="6bf74-106">תיעוד תחת [תחומים של Yammer ו-Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) זמין.</span><span class="sxs-lookup"><span data-stu-id="6bf74-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="6bf74-107">הסיבה הנפוצה ביותר שבגללה אתה רואה תחום שגוי היא שקיימות רשתות Yammer מרובות ויש לאחד אותן.</span><span class="sxs-lookup"><span data-stu-id="6bf74-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="6bf74-108">[איחוד לרשת אחת](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) באמצעות כלי ההעברה של הרשת הוא שלב ראשון חשוב.</span><span class="sxs-lookup"><span data-stu-id="6bf74-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="6bf74-109">השלם אותו לפני שתנסה להגדיר את התחום הראשי שלך.</span><span class="sxs-lookup"><span data-stu-id="6bf74-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="6bf74-110">**אין תחומים מותאמים אישית**</span><span class="sxs-lookup"><span data-stu-id="6bf74-110">**No custom domains**</span></span>

<span data-ttu-id="6bf74-111">עבור דיירים חדשים, תחום ברירת המחדל (לדוגמה fabrikam.onmicrosoft.com) מהדייר ישמש עבור Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bf74-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="6bf74-112">התחום הראשי מוגדר אל yammer.com/fabrikam.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="6bf74-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="6bf74-113">**תחום מותאם אישית יחיד**</span><span class="sxs-lookup"><span data-stu-id="6bf74-113">**Single custom domain**</span></span>

<span data-ttu-id="6bf74-114">Yammer תבחר באופן אוטומטי את תחום ברירת המחדל (לדוגמה fabrikam.com) מהדייר כתחום הראשי ב- Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bf74-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="6bf74-115">הוא מוגדר אל yammer.com/fabrikam.com.</span><span class="sxs-lookup"><span data-stu-id="6bf74-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="6bf74-116">שינוי זה מבוצע על-ידי שירות סנכרון התחום, ועלול להימשך עד 24 שעות כדי להיכנס לתוקף.</span><span class="sxs-lookup"><span data-stu-id="6bf74-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="6bf74-117">**תחומים מותאמים אישית מרובים**</span><span class="sxs-lookup"><span data-stu-id="6bf74-117">**Multiple custom domains**</span></span>

<span data-ttu-id="6bf74-118">ל- Yammer יכול להיות תחום ראשי שונה מתחום ברירת המחדל של דייר.</span><span class="sxs-lookup"><span data-stu-id="6bf74-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="6bf74-119">מכיוון שיש תחומים מותאמים אישית מרובים, Yammer לא מנסה לנחש את התחום הנכון מבין התחומים הזמינים.</span><span class="sxs-lookup"><span data-stu-id="6bf74-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="6bf74-120">עליך לפתוח מקרה תמיכה כדי לבקש לשנו את שם התחום הראשי לתחום הראשי שבחרת.</span><span class="sxs-lookup"><span data-stu-id="6bf74-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="6bf74-121">**מידע נוסף לפתרון בעיות**</span><span class="sxs-lookup"><span data-stu-id="6bf74-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="6bf74-122">במקרים מסומים, ייתכן שתחומים הועברו בין דיירים ולשירות הסנכרון של תחום לא הייתה יכולת לפעול בהצלחה.</span><span class="sxs-lookup"><span data-stu-id="6bf74-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="6bf74-123">ייתכן שתחווה בעיות כניסה או בעיות אחרות, בנוסף לתחום ראשי שגוי.</span><span class="sxs-lookup"><span data-stu-id="6bf74-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="6bf74-124">כדי לפתור בעיה זו, ייתכן שיהיה להעביר את התחומים אל הרשת הנכונה בעזרת התמיכה של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6bf74-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="6bf74-125">פתרון זה דורש סיוע ישיר ועשוי להימשך זמן מה, במיוחד אם יש רשימת ארוכה מאוד של שמות תחומים.</span><span class="sxs-lookup"><span data-stu-id="6bf74-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="6bf74-126">פתח מקרה תמיכה כדי לקבל סיוע בפתרון של סוגי בעיות אלה.</span><span class="sxs-lookup"><span data-stu-id="6bf74-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="6bf74-127">בעת עבודה עם נציג תמיכה, הוא יבדוק שהתחומים מאומתים בדייר תחת שליטתך.</span><span class="sxs-lookup"><span data-stu-id="6bf74-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="6bf74-128">ייתכן שהוא ישאל שאלות אימות נוספות בנוגע לתחומים שלך אם הם נוספים לדייר שלך אך אינם מאומתים על-ידי DNS.</span><span class="sxs-lookup"><span data-stu-id="6bf74-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="6bf74-129">ודא שהתחומים מאומתים על-ידי DNS כדי לזרז את התהליך.</span><span class="sxs-lookup"><span data-stu-id="6bf74-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
