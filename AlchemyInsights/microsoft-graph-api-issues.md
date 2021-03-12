---
title: בעיות API של Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713704"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="2e7b3-102">בעיות API של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="2e7b3-103">נושא זה עשוי גם לחול על מפתחים שעדיין משתמשים ב-API של הודעות מיידיות של גרף.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="2e7b3-104">עם זאת, מומלץ **מאוד** להשתמש ב-Microsoft Graph עבור כל תרחישי הספריה, הזהות וניהול הגישה שלך.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="2e7b3-105">**בעיות אימות או הרשאה**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="2e7b3-106">אם היישום שלך אינו **מצליח לרכוש אסימונים** לצורך התקשרות ל-microsoft graph, בחר **בעיה בקבלת הקטגוריה ' אסימון גישה ' (אימות)** microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="2e7b3-107">אם האפליקציה שלך **מקבלת שגיאות הרשאה של 401 או 403** בעת התקשרות ל-microsoft graph, בחר את הקטגוריה **קבלת שגיאה של microsoft graph שנדחתה (הרשאה)** של microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="2e7b3-108">**אני מעוניין להשתמש ב-Microsoft Graph, אך לא בטוח היכן להתחיל**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="2e7b3-109">מבט כולל על Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="2e7b3-110">מבט כולל על זהות וניהול גישה ב-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="2e7b3-111">תחילת הבנייה של יישומי Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="2e7b3-112">**סייר Microsoft graph** -בדיקת ממשקי Api של microsoft graph בדייר שלך או בדייר הדגמה</span><span class="sxs-lookup"><span data-stu-id="2e7b3-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="2e7b3-113">**אני מעוניין להשתמש ב-Microsoft Graph, אך האם היא תומכת בממשקי Api של מדריכי כתובות של v 1.0 שאני זקוק להם?**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="2e7b3-114">Microsoft Graph הוא ה-API המומלץ עבור מדריכי כתובות, זהויות וניהול גישה.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="2e7b3-115">עם זאת, עדיין קיימים כמה פערים בין מה שאפשרי באזור התכלת והגרפי של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="2e7b3-116">סקור את המאמרים הבאים, אשר מדגישים את ההבדלים העדכניים ביותר כדי לסייע בבחירתך:</span><span class="sxs-lookup"><span data-stu-id="2e7b3-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="2e7b3-117">הבדלים בין סוגי משאבים בין מע וגרף של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="2e7b3-118">הבדלים בין המאפיינים של ' תכלת והגרף ' ל-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="2e7b3-119">הבדלי שיטות בין תכלת לספירה ל-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="2e7b3-120">**ממשק ה-API שאני מתקשר אליו אינו פועל-היכן ניתן לבצע בדיקות נוספות?**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="2e7b3-121">**סייר Microsoft graph** -בדוק את ממשקי ה-Api של microsoft graph בדייר שלך או בדייר הדגמה ועיין גם **בשאילתות לדוגמה** ב-Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="2e7b3-122">**האפליקציה שלי איטית מדי והיא מקבלת מצערת גם כן. אילו שיפורים ניתן לעשות?**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="2e7b3-123">בהתאם לתרחיש שלך, קיימות מגוון אפשרויות לשירותך כדי להפוך את היישום שלך לביצועים טובים יותר, ובמקרים מסוימים, להיות פחות מועדים לוויסות השירות (כאשר אתה מבצע שיחות רבות מדי).</span><span class="sxs-lookup"><span data-stu-id="2e7b3-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="2e7b3-124">שיטות העבודה המומלצות של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="2e7b3-125">בקשות לאצווה</span><span class="sxs-lookup"><span data-stu-id="2e7b3-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="2e7b3-126">מעקב אחר שינויים בשאילתת דלתא</span><span class="sxs-lookup"><span data-stu-id="2e7b3-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="2e7b3-127">קבל הודעה על שינויים באמצעות webhooks</span><span class="sxs-lookup"><span data-stu-id="2e7b3-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="2e7b3-128">הדרכה בוויסות</span><span class="sxs-lookup"><span data-stu-id="2e7b3-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="2e7b3-129">**היכן ניתן למצוא מידע נוסף אודות שגיאות ובעיות ידועות?**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="2e7b3-130">מידע אודות תגובת השגיאה של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="2e7b3-131">בעיות ידועות ב-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7b3-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="2e7b3-132">**היכן ניתן לבדוק את מצב הזמינות והקישוריות של שירות?**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="2e7b3-133">זמינות השירות והקישוריות של השירותים המשמשים כבסיס אליהם ניתן לגשת דרך Microsoft Graph יכולה להשפיע על הזמינות והביצועים הכוללים של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="2e7b3-134">לקבלת התקינות של שירות השירות של Active Directory, בדוק את מצב **האבטחה +** שירותי זהויות המפורטים [בדף ' מצב תכלת](https://azure.microsoft.com/status/)'.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="2e7b3-135">עבור שירותי Office התורמים ל-Microsoft Graph, בדוק את מצב השירותים המפורטים [בלוח המחוונים של תקינות השירות של Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="2e7b3-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="2e7b3-136">שגיאות הרשאה של Microsoft Graph עשויות לנבוע ממספר בעיות שונות, שרובו מפיק שגיאת 401 או 403.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="2e7b3-137">לדוגמה, הגורמים הבאים יכולים להוביל לשגיאות הרשאה:</span><span class="sxs-lookup"><span data-stu-id="2e7b3-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="2e7b3-138">[זרימות רכישה שגויות של אסימוני גישה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="2e7b3-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="2e7b3-139">[טווחי הרשאות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) שתצורתם לא נקבעה כהלכה</span><span class="sxs-lookup"><span data-stu-id="2e7b3-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="2e7b3-140">היעדר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="2e7b3-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="2e7b3-141">\**_סיום התמיכה עבור ספריית האימות של Azure Active Directory ‏(ADAL) ועבור ה- API של Azure AD Graph ‏(AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="2e7b3-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="2e7b3-142">_ \* החל מ-30 ביוני, 2020 \* \*, לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="2e7b3-143">נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="2e7b3-144">**החל מ-30 ביוני 2022**, נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="2e7b3-145">יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא *יקבלו שום תמיכה טכנית או עדכוני אבטחה*.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="2e7b3-146">יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="2e7b3-147">**העברת ADAL**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-147">**ADAL Migration**</span></span>

<span data-ttu-id="2e7b3-148">אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="2e7b3-149">אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי תאריך היעד של סיום התמיכה, ומבטיחה שיפיקו תועלת מהשיפורים המתמשכים של האבטחה והתכונות של MSAL.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="2e7b3-150">קרא את השאלות הנפוצות בנושא ADAL</span><span class="sxs-lookup"><span data-stu-id="2e7b3-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="2e7b3-151">למד כיצד להעביר אפליקציות לפי פלטפורמה</span><span class="sxs-lookup"><span data-stu-id="2e7b3-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="2e7b3-152">אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="2e7b3-153">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="2e7b3-154">**העברת AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="2e7b3-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="2e7b3-155">עבור יישומים המשתמשים ב-תכלת AD Graph, בצע את ההנחיות שלנו כדי [להעביר את האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="2e7b3-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="2e7b3-156">[רשימת הפעולות לביצוע של ההעברה מספקת נקודת פתיחה לתחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="2e7b3-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="2e7b3-157">פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="2e7b3-158">אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="2e7b3-159">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל השימוש בגרף של ה-עמ-שימוש בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="2e7b3-160">כדי שהיישום שלך ייגש לנתונים ב-Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="2e7b3-161">[ההפניה להרשאות Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) מפרטת את ההרשאות המשויכות לכל קבוצה עיקרית של ממשקי Api של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="2e7b3-162">כמו כן, הוא מספק הנחיות לגבי אופן השימוש בהרשאות.</span><span class="sxs-lookup"><span data-stu-id="2e7b3-162">It also provides guidance about how to use the permissions.</span></span>
