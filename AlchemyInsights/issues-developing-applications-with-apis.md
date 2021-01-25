---
title: בעיות בפיתוח יישומים באמצעות APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974619"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="03109-102">בעיות בפיתוח יישומים באמצעות APIs</span><span class="sxs-lookup"><span data-stu-id="03109-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="03109-103">כדי להתחיל להשתמש ב-API של מדריכי כתובות ב-API של Active Directory, עיין [במדריך ההדרכה של הודעות מיידיות](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ב-api של תחלה, או הצג את [התיעוד האינטראקטיבי של ההפניה לשימוש](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)ב</span><span class="sxs-lookup"><span data-stu-id="03109-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="03109-104">**סיום התמיכה עבור ממשק האימות של מדריכי כתובות של Active Directory (ADAL) ו-active AD Graph API (הגרף עמ מ)**</span><span class="sxs-lookup"><span data-stu-id="03109-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="03109-105">**החל מ-30 ביוני, 2020**, לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph.</span><span class="sxs-lookup"><span data-stu-id="03109-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="03109-106">אנו נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא ניתן עוד לספק עדכוני תכונות.</span><span class="sxs-lookup"><span data-stu-id="03109-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="03109-107">**החל מ-30 ביוני 2022**, נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="03109-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="03109-108">יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא יקבלו שום תמיכה טכנית או עדכוני אבטחה.</span><span class="sxs-lookup"><span data-stu-id="03109-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="03109-109">יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.</span><span class="sxs-lookup"><span data-stu-id="03109-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="03109-110">**העברת ADAL**</span><span class="sxs-lookup"><span data-stu-id="03109-110">**ADAL Migration**</span></span>

<span data-ttu-id="03109-111">מומלץ לעדכן את [ספריית האימות של Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה העדכניים ביותר.</span><span class="sxs-lookup"><span data-stu-id="03109-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="03109-112">אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי תאריך היעד של סיום התמיכה, ומבטיחה שיפיקו תועלת מהשיפורים המתמשכים של האבטחה והתכונות של MSAL.</span><span class="sxs-lookup"><span data-stu-id="03109-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="03109-113">[קרא את השאלות הנפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="03109-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="03109-114">[למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="03109-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="03109-115">אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים.</span><span class="sxs-lookup"><span data-stu-id="03109-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="03109-116">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל היישומים שאינם של Microsoft ADAL בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="03109-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="03109-117">**העברת גרף מ-עמ**</span><span class="sxs-lookup"><span data-stu-id="03109-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="03109-118">עבור יישומים המשתמשים ב-תכלת AD Graph, בצע את ההנחיות שלנו כדי להעביר את [האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="03109-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="03109-119">[רשימת הפעולות לביצוע של ההעברה מספקת נקודת תחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="03109-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="03109-120">פורטל הרישום של האפליקציה ' תכלת ' מראה אילו יישומים משתמשים ב-עמ-גרף.</span><span class="sxs-lookup"><span data-stu-id="03109-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="03109-121">אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים.</span><span class="sxs-lookup"><span data-stu-id="03109-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="03109-122">התמיכה של Microsoft יכולה גם לספק לך רשימה של כל השימוש בגרף של ה-עמ-שימוש בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="03109-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="03109-123">כדי שהיישום שלך ייגש לנתונים ב-Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה.</span><span class="sxs-lookup"><span data-stu-id="03109-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="03109-124">[ההפניה להרשאות Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) מפרטת את ההרשאות המשויכות לכל קבוצה עיקרית של ממשקי Api של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="03109-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="03109-125">כמו כן, הוא מספק הנחיות לגבי אופן השימוש בהרשאות.</span><span class="sxs-lookup"><span data-stu-id="03109-125">It also provides guidance about how to use the permissions.</span></span>
