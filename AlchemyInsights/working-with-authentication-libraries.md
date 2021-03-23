---
title: עבודה עם ספריות אימות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035831"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="36491-102">עבודה עם ספריות אימות</span><span class="sxs-lookup"><span data-stu-id="36491-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="36491-103">כדי לפתור בעיה בספריית האימות של Microsoft (MSAL), בצע את השלבים המומלצים הבאים:</span><span class="sxs-lookup"><span data-stu-id="36491-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="36491-104">**עבודה עם MSAL**: [ספריות אימות של פלטפורמת הזהויות של microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -מאמר זה מציג את התמיכה בספריית האימות של microsoft עבור כמה סוגי יישומים.</span><span class="sxs-lookup"><span data-stu-id="36491-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="36491-105">הוא כולל קישורים לקוד מקור ספריה; היכן לקבל את החבילה עבור הפרוייקט של היישום; והאם הספריה תומכת בכניסה למשתמש (אימות), גישה לממשקי אינטרנט מוגנים (אישור), או שתיהן.</span><span class="sxs-lookup"><span data-stu-id="36491-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="36491-106">**פתרון בעיות באימות**: הMSAL תומך במספר זרימות אימות לשימוש בתרחישים שונים של יישומים.</span><span class="sxs-lookup"><span data-stu-id="36491-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="36491-107">בהתאם לאופן הבנייה של יישום הלקוח שלך, MSAL יכול להשתמש באחד או יותר מזרמי האימות הנתמכים על-ידי פלטפורמת הזהות של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="36491-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="36491-108">זרימות אלה יכולות ליצור מספר סוגים של אסימונים וקודי הרשאות, ולדרוש אסימונים שונים כדי לגרום להם לפעול.</span><span class="sxs-lookup"><span data-stu-id="36491-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="36491-109">**אסימוני גישה**: [אסימוני גישה של פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -למד כיצד ה-API שלך יכול לאמת ולהשתמש בטענות בתוך אסימון גישה.</span><span class="sxs-lookup"><span data-stu-id="36491-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="36491-110">כל התיעוד במאמר זה, למעט היכן שצוין, חל רק על אסימונים שהונפקו עבור APIs שנרשמת.</span><span class="sxs-lookup"><span data-stu-id="36491-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="36491-111">הוא אינו חל על אסימונים שהונפקו עבור ממשקי Api בבעלות Microsoft, וגם לא ניתן להשתמש באסימונים אלה כדי לאמת את האופן שבו פלטפורמת הזהות של Microsoft תיצור אסימונים עבור ממשק API שאתה יוצר.</span><span class="sxs-lookup"><span data-stu-id="36491-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="36491-112">**סיום התמיכה בספריית האימות של Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="36491-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="36491-113">**החל מ-30 ביוני, 2020,** לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph.</span><span class="sxs-lookup"><span data-stu-id="36491-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="36491-114">נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.</span><span class="sxs-lookup"><span data-stu-id="36491-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="36491-115">**החל מ-30 ביוני 2022,** נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="36491-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="36491-116">יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא *יקבלו שום תמיכה טכנית או עדכוני אבטחה*.</span><span class="sxs-lookup"><span data-stu-id="36491-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="36491-117">יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.</span><span class="sxs-lookup"><span data-stu-id="36491-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="36491-118">**העברת ADAL**</span><span class="sxs-lookup"><span data-stu-id="36491-118">**ADAL Migration**</span></span>

- <span data-ttu-id="36491-119">מומלץ לעדכן את MSAL, הכולל את התכונות ועדכוני האבטחה העדכניים ביותר.</span><span class="sxs-lookup"><span data-stu-id="36491-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="36491-120">אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי מועד היעד של סוף התמיכה, ומבטיחה שייהנו מהאבטחה המתמשכת של MSAL ושיפורים בתכונות.</span><span class="sxs-lookup"><span data-stu-id="36491-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="36491-121">[קרא את השאלות הנפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="36491-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="36491-122">[למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="36491-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="36491-123">אם לאחר קריאת המדריך לפלטפורמת האפליקציה שלך, יש לך שאלות נוספות, באפשרותך לפרסם ב- [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) עם התגית [תכלת-ad-adal-תבטלות] או לפתוח בעיה במאגר GitHub של הספריה.</span><span class="sxs-lookup"><span data-stu-id="36491-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="36491-124">עיין במקטע [שפות ומסגרות](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) של מאמר **מבט כולל של MSAL** עבור קישורים לכל מספר ריפו של ספריה.</span><span class="sxs-lookup"><span data-stu-id="36491-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="36491-125">**אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL**, אנו ממליצים לך לסקור את כל קוד המקור של היישומים שלך.</span><span class="sxs-lookup"><span data-stu-id="36491-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="36491-126">במידת הצורך, הושיטו יד לספקי תוכנה עצמאיים (Isv) או לספקי יישומים.</span><span class="sxs-lookup"><span data-stu-id="36491-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="36491-127">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="36491-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







