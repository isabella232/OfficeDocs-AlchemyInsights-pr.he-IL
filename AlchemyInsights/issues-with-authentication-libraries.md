---
title: בעיות בספריות אימות
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063608"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="c08f5-102">בעיות בספריות אימות</span><span class="sxs-lookup"><span data-stu-id="c08f5-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="c08f5-103">[ספריות האימות של פלטפורמת הזהויות של microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) מפרטות את הספריות הנתמכות והתווכה של microsoft ללקוחות ולקוחות שתואמים</span><span class="sxs-lookup"><span data-stu-id="c08f5-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="c08f5-104">ספריית האימות של Microsoft (MSAL) תומכת במספר [זרימות אימות](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) לשימוש בתרחישים שונים של יישומים.</span><span class="sxs-lookup"><span data-stu-id="c08f5-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="c08f5-105">כדי לאמת ולרכוש אסימונים, עליך לאתחל יישום לקוח ציבורי או סודי חדש בקוד שלך.</span><span class="sxs-lookup"><span data-stu-id="c08f5-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="c08f5-106">באפשרותך להגדיר כמה אפשרויות תצורה בעת אתחול יישום הלקוח בספריית האימות של Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="c08f5-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="c08f5-107">לקבלת מידע נוסף, ראה [אפשרויות תצורת יישום](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="c08f5-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="c08f5-108">**סיום התמיכה עבור ממשק האימות של מדריכי כתובות של Active Directory (ADAL) ו-active AD Graph API (הגרף עמ מ)**</span><span class="sxs-lookup"><span data-stu-id="c08f5-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="c08f5-109">**החל מ-30 ביוני, 2020**, לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph.</span><span class="sxs-lookup"><span data-stu-id="c08f5-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="c08f5-110">נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.</span><span class="sxs-lookup"><span data-stu-id="c08f5-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="c08f5-111">**החל מ-30 ביוני 2022**, נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="c08f5-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="c08f5-112">יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא *יקבלו שום תמיכה טכנית או עדכוני אבטחה*.</span><span class="sxs-lookup"><span data-stu-id="c08f5-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="c08f5-113">יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.</span><span class="sxs-lookup"><span data-stu-id="c08f5-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="c08f5-114">**העברת ADAL**</span><span class="sxs-lookup"><span data-stu-id="c08f5-114">**ADAL Migration**</span></span>

<span data-ttu-id="c08f5-115">אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.</span><span class="sxs-lookup"><span data-stu-id="c08f5-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="c08f5-116">אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי תאריך היעד של סיום התמיכה, ולהבטיח שייהנו מהשיפור המתמשך של האבטחה והתכונות של MSAL.</span><span class="sxs-lookup"><span data-stu-id="c08f5-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="c08f5-117">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="c08f5-117">For more information, see:</span></span>

1. [<span data-ttu-id="c08f5-118">קרא את השאלות הנפוצות בנושא ADAL</span><span class="sxs-lookup"><span data-stu-id="c08f5-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="c08f5-119">למד כיצד להעביר אפליקציות לפי פלטפורמה</span><span class="sxs-lookup"><span data-stu-id="c08f5-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="c08f5-120">אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים.</span><span class="sxs-lookup"><span data-stu-id="c08f5-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="c08f5-121">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="c08f5-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="c08f5-122">**העברת AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="c08f5-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="c08f5-123">עבור יישומים המשתמשים ב-תכלת AD Graph, בצע את ההנחיות שלנו כדי [להעביר את האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="c08f5-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="c08f5-124">רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה.</span><span class="sxs-lookup"><span data-stu-id="c08f5-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="c08f5-125">פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="c08f5-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="c08f5-126">אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="c08f5-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="c08f5-127">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל השימוש בגרף של ה-עמ-שימוש בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="c08f5-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="c08f5-128">כדי שהיישום שלך ייגש לנתונים ב-Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה.</span><span class="sxs-lookup"><span data-stu-id="c08f5-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="c08f5-129">[ההפניה להרשאות Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) מפרטת את ההרשאות המשויכות לכל קבוצה עיקרית של ממשקי Api של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c08f5-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="c08f5-130">כמו כן, הוא מספק הנחיות לגבי אופן השימוש בהרשאות.</span><span class="sxs-lookup"><span data-stu-id="c08f5-130">It also provides guidance about how to use the permissions.</span></span>
