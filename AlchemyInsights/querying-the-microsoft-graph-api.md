---
title: שאילתה ב-API של Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974419"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="1fcb9-102">שאילתה ב-API של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="1fcb9-103">נושא זה עשוי גם לחול על מפתחים שעדיין משתמשים ב-API של הודעות מיידיות של גרף.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="1fcb9-104">עם זאת, מומלץ **מאוד** להשתמש ב-Microsoft Graph עבור כל תרחישי הספריה, הזהות וניהול הגישה שלך.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="1fcb9-105">**בעיות אימות או הרשאה**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="1fcb9-106">אם היישום שלך אינו **מצליח לרכוש אסימונים** לצורך התקשרות ל-microsoft graph, בחר **בעיה בקבלת הקטגוריה ' אסימון גישה ' (אימות)** microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="1fcb9-107">אם האפליקציה שלך **מקבלת שגיאות הרשאה של 401 או 403** בעת התקשרות ל-microsoft graph, בחר את הקטגוריה **קבלת שגיאה של microsoft graph שנדחתה (הרשאה)** של microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="1fcb9-108">**אני מעוניין להשתמש ב-Microsoft Graph, אך לא בטוח היכן להתחיל**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="1fcb9-109">לקבלת מידע נוסף אודות Microsoft Graph, ראה:</span><span class="sxs-lookup"><span data-stu-id="1fcb9-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="1fcb9-110">מבט כולל על Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="1fcb9-111">מבט כולל על זהות וניהול גישה ב-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="1fcb9-112">תחילת הבנייה של יישומי Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="1fcb9-113">**סייר Microsoft graph** -בדיקת ממשקי Api של microsoft graph בדייר שלך או בדייר הדגמה</span><span class="sxs-lookup"><span data-stu-id="1fcb9-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="1fcb9-114">**אני מעוניין להשתמש ב-Microsoft Graph, אך האם היא תומכת בממשקי Api של מדריכי כתובות של v 1.0 שאני זקוק להם?**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="1fcb9-115">Microsoft Graph הוא ה-API המומלץ עבור מדריכי כתובות, זהויות וניהול גישה.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="1fcb9-116">עם זאת, עדיין קיימים כמה פערים בין מה שאפשרי באזור התכלת והגרפי של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="1fcb9-117">סקור את המאמרים הבאים, אשר מדגישים את ההבדלים העדכניים ביותר כדי לסייע בבחירתך:</span><span class="sxs-lookup"><span data-stu-id="1fcb9-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="1fcb9-118">הבדלים בין סוגי משאבים בין מע וגרף של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="1fcb9-119">הבדלים בין המאפיינים של ' תכלת והגרף ' ל-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="1fcb9-120">הבדלי שיטות בין תכלת לספירה ל-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="1fcb9-121">**כאשר אני מבצע שאילתה על אובייקט *המשתמש* , רבים מהמאפיינים שלו חסרים**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="1fcb9-122">`GET https://graph.microsoft.com/v1.0/users` הפונקציה מחזירה רק 11 מאפיינים, מאחר ש-Microsoft Graph בוחר באופן אוטומטי קבוצת מאפיינים של *משתמש* שברצונך להחזיר.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="1fcb9-123">אם אתה זקוק למאפייני *משתמש* אחרים, השתמש ב$select כדי לבחור את המאפיינים הדרושים ליישום שלך.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="1fcb9-124">נסה זאת **בסייר Microsoft Graph** תחילה.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="1fcb9-125">**ערכי מאפיינים מסוימים של משתמשים הם *null* למרות שאני יודע שהם מוגדרים**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="1fcb9-126">ההסבר הסביר ביותר הוא שהיישום הוענקה *למשתמש. ReadBasic. All* הרשאה.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="1fcb9-127">פעולה זו מאפשרת ליישום לקרוא קבוצה מוגבלת של מאפייני משתמש, ולהחזיר את כל המאפיינים האחרים כערכי null גם אם הם הוגדרו בעבר.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="1fcb9-128">נסה להעניק *למשתמש היישום. קרא את כל* ההרשאות במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="1fcb9-129">לקבלת מידע נוסף, ראה [הרשאות משתמש של Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="1fcb9-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="1fcb9-130">**אני נתקל בבעיות בשימוש בפרמטרי שאילתות של OData כדי לסנן נתונים בבקשות שלי**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="1fcb9-131">בעוד ש-Microsoft Graph תומך בטווח רחב של הפרמטרים של שאילתת OData, רבים מהפרמטרים האלה אינם נתמכים באופן מלא על-ידי שירותי מדריך כתובות (משאבים היורשים מ- *directoryObject*) ב-Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="1fcb9-132">אותן מגבלות שהיו קיימות ב-תכלת AD Graph נמשכות ברוב המקרים ב-Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="1fcb9-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="1fcb9-133">**לא נתמך**: $count, $search ו$filter *בערכי null* או *Not null*</span><span class="sxs-lookup"><span data-stu-id="1fcb9-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="1fcb9-134">**לא נתמך**: $filter במאפיינים מסוימים (ראה נושאי משאבים שעליהם ניתן לסנן מאפיינים)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="1fcb9-135">**לא נתמך**: קידוד, סינון ומיון בו</span><span class="sxs-lookup"><span data-stu-id="1fcb9-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="1fcb9-136">**לא נתמך**: סינון בקשר גומלין.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="1fcb9-137">לדוגמה-חיפוש כל החברים בקבוצת ההנדסה הנמצאים בבריטניה.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="1fcb9-138">**תמיכה חלקית**: $orderby ב- *user* (displayName ו-userPrincipalName בלבד) *וקבוצה*</span><span class="sxs-lookup"><span data-stu-id="1fcb9-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="1fcb9-139">**תמיכה חלקית**: $filter (תומך רק ב- *eq*, ב- *startswith* *או* ב- *and* ובתמיכה *מוגבלת)*, $expand (הרחבת קשרי הגומלין של אובייקט יחיד מחזירה את כל קשרי הגומלין, אך הרחבת אוסף של קשרי גומלין היא מוגבלת)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="1fcb9-140">לקבלת מידע נוסף, ראה [התאמה אישית של תגובות באמצעות פרמטרי שאילתה](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1fcb9-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="1fcb9-141">**ה-API שאני מתקשר אליו אינו פועל-היכן ניתן לבצע בדיקות נוספות?**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="1fcb9-142">**סייר Microsoft graph** -בדוק את ממשקי ה-Api של microsoft graph בדייר שלך או בדייר הדגמה ועיין גם **בשאילתות לדוגמה** ב-Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="1fcb9-143">**כאשר אני מבצע שאילתה עבור נתונים, נראה שאני מקבל בחזרה הגדרת נתונים לא מלאה**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="1fcb9-144">אם אתה מבצע שאילתה על אוסף (כגון *משתמשים*), Microsoft Graph משתמש במגבלות עמוד בצד השרת, כך שהתוצאות יוחזרו תמיד עם גודל עמוד המוגדר כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="1fcb9-145">היישום שלך אמור תמיד לצפות לעמוד באמצעות אוספים המוחזרים מהשירות.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="1fcb9-146">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="1fcb9-146">For more information, see:</span></span>

- [<span data-ttu-id="1fcb9-147">שיטות העבודה המומלצות של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1fcb9-148">החלפת נתונים של Microsoft Graph באפליקציה</span><span class="sxs-lookup"><span data-stu-id="1fcb9-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="1fcb9-149">**האפליקציה שלי איטית מדי והיא מקבלת מצערת גם כן. אילו שיפורים ניתן לעשות?**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="1fcb9-150">בהתאם לתרחיש שלך, קיימות מגוון אפשרויות שונות לרשותכם כדי להפוך את היישום שלך לביצועים טובים יותר, ובמקרים מסוימים, פחות מועדים לשימוש מצערת על-ידי השירות (כאשר אתה מבצע שיחות רבות מדי).</span><span class="sxs-lookup"><span data-stu-id="1fcb9-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="1fcb9-151">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="1fcb9-151">To learn more, see:</span></span>

- [<span data-ttu-id="1fcb9-152">שיטות העבודה המומלצות של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1fcb9-153">בקשות לאצווה</span><span class="sxs-lookup"><span data-stu-id="1fcb9-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="1fcb9-154">מעקב אחר שינויים בשאילתת דלתא</span><span class="sxs-lookup"><span data-stu-id="1fcb9-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="1fcb9-155">קבל הודעה על שינויים באמצעות webhooks</span><span class="sxs-lookup"><span data-stu-id="1fcb9-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="1fcb9-156">הדרכה בוויסות</span><span class="sxs-lookup"><span data-stu-id="1fcb9-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="1fcb9-157">**היכן ניתן למצוא מידע נוסף אודות שגיאות ובעיות ידועות?**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="1fcb9-158">מידע אודות תגובת השגיאה של Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="1fcb9-159">בעיות ידועות ב-Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fcb9-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="1fcb9-160">**היכן ניתן לבדוק את מצב הזמינות והקישוריות של שירות?**</span><span class="sxs-lookup"><span data-stu-id="1fcb9-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="1fcb9-161">זמינות השירות והקישוריות של השירותים המשמשים כבסיס אליהם ניתן לגשת דרך Microsoft Graph יכולה להשפיע על הזמינות והביצועים הכוללים של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="1fcb9-162">לקבלת התקינות של שירות השירות של Active Directory, בדוק את מצב **האבטחה +** שירותי זהויות המפורטים [בדף ' מצב תכלת](https://azure.microsoft.com/status/)'.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="1fcb9-163">עבור שירותי Office התורמים ל-Microsoft Graph, בדוק את מצב השירותים המפורטים [בלוח המחוונים של תקינות השירות של Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1fcb9-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
