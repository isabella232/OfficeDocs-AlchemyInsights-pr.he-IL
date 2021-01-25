---
title: בעיות בפיתוח יישומים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974474"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="4880b-102">בעיות בפיתוח יישומים</span><span class="sxs-lookup"><span data-stu-id="4880b-102">Issues developing applications</span></span>

<span data-ttu-id="4880b-103">כדי לפתור את הבעיות הנפוצות ביותר בעת בניית יישומי תכלת של Active Directory (AD), עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="4880b-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="4880b-104">אני רואה בעיות כניסה ליישומים באמצעות דפדפן Chrome בלבד</span><span class="sxs-lookup"><span data-stu-id="4880b-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="4880b-105">איני יודע כיצד לשנות את ברירות המחדל של כל החיים של האסימון עבור היישום שלי</span><span class="sxs-lookup"><span data-stu-id="4880b-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="4880b-106">אני מבולבל לגבי אופן הפעולה של הסכמת היישום</span><span class="sxs-lookup"><span data-stu-id="4880b-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="4880b-107">איני יודע כיצד להעניק הרשאות ליישום שלי</span><span class="sxs-lookup"><span data-stu-id="4880b-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="4880b-108">איני מבין את ההבדל בין הרשאות מוקצות והרשאות יישום</span><span class="sxs-lookup"><span data-stu-id="4880b-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="4880b-109">\***סיום התמיכה עבור כללי האימות של מדריכי הכתובות של Active Directory (ADAL) וממשק תכלת של הודעות מיידיות ב-API (הגרף עמ מ)** _</span><span class="sxs-lookup"><span data-stu-id="4880b-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="4880b-110">החל מ-30 ביוני, 2020, לא נוסיף עוד תכונות חדשות לספריית האימות של Active Directory (ADAL) והתכלת הגרפי של הודעות מיידיות (API).</span><span class="sxs-lookup"><span data-stu-id="4880b-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="4880b-111">אנו נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא ניתן עוד לספק עדכוני תכונות.</span><span class="sxs-lookup"><span data-stu-id="4880b-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="4880b-112">החל מ-30 ביוני 2022, אנו נסיים את התמיכה עבור ADAL ו-עמ-עמ והוא לא יספק עוד תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="4880b-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="4880b-113">כתוצאה מתנאי זה, להלן ההשלכות:</span><span class="sxs-lookup"><span data-stu-id="4880b-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="4880b-114">יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא יקבלו שום תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="4880b-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="4880b-115">יישומים באמצעות גרף עמ-משתמשים לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של גרף ה-עמ</span><span class="sxs-lookup"><span data-stu-id="4880b-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="4880b-116">_ *העברה של ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="4880b-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="4880b-117">אם אתה משתמש ב-Microsoft apps, מומלץ לעדכן לספריית האימות של Microsoft (MSAL), הכוללת את התכונות ועדכוני האבטחה העדכניים ביותר.</span><span class="sxs-lookup"><span data-stu-id="4880b-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="4880b-118">המלצה זו נמצאת בהקשר של Microsoft היוזמת את תהליך העברת האפליקציות שלה ל-MSAL על-ידי מועד היעד של סוף התמיכה.</span><span class="sxs-lookup"><span data-stu-id="4880b-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="4880b-119">ההעברה על-ידי Microsoft של היישומים שלה ל-MSAL מבטיחה שהיישומים ירוויחו מהאבטחה המתמשכת של MSAL ושיפורים בתכונות.</span><span class="sxs-lookup"><span data-stu-id="4880b-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="4880b-120">קריאת השאלות הנפוצות של ADAL</span><span class="sxs-lookup"><span data-stu-id="4880b-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="4880b-121">למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה</span><span class="sxs-lookup"><span data-stu-id="4880b-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="4880b-122">אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים שלך, ובמידת הצורך, להושיט יד לכל ספקי תוכנה עצמאיים (Isv) או לספקי יישומים.</span><span class="sxs-lookup"><span data-stu-id="4880b-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="4880b-123">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל היישומים שאינם של Microsoft ADAL בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="4880b-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="4880b-124">**העברת גרף מ-עמ**</span><span class="sxs-lookup"><span data-stu-id="4880b-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="4880b-125">עבור יישומים המשתמשים בגרף של ה-עמ, פעל לפי ההנחיות שלנו כדי להעביר את האפליקציות של גרף עמ ' ל-Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="4880b-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="4880b-126">[רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="4880b-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="4880b-127">פורטל הרישום של האפליקציה ' תכלת ' מראה אילו יישומים משתמשים ב-עמ-גרף.</span><span class="sxs-lookup"><span data-stu-id="4880b-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="4880b-128">אנו ממליצים לך לסקור את כל קוד המקור של היישומים שלך, ובמידת הצורך, להושיט יד לכל ספקי תוכנה עצמאיים (Isv) או לספקי יישומים.</span><span class="sxs-lookup"><span data-stu-id="4880b-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="4880b-129">התמיכה של Microsoft יכולה גם לספק לך מידע אודות השימוש בגרף של שימוש בגרף של הדייר.</span><span class="sxs-lookup"><span data-stu-id="4880b-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







