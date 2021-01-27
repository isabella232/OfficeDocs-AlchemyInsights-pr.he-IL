---
title: בעיות גישה מותנית
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014882"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="e61b8-102">בעיות גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="e61b8-102">Conditional access issues</span></span>

<span data-ttu-id="e61b8-103">**פתרון בעיות באבחון הכניסה**</span><span class="sxs-lookup"><span data-stu-id="e61b8-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="e61b8-104">באפשרותך לגלות במהירות מה קרה או לאבחן בעיות הקשורות לכניסה למשתמש באמצעות [אבחון הכניסה](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="e61b8-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="e61b8-105">הפעל את אבחון הכניסה.</span><span class="sxs-lookup"><span data-stu-id="e61b8-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="e61b8-106">אתר את האירוע לניתוח על-ידי הזנת הפרטים שאתה משתמש בהם לגבי המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.</span><span class="sxs-lookup"><span data-stu-id="e61b8-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="e61b8-107">סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואילו פעולות ניתן לבצע כדי לבצע שינויים (אם נדרשים שינויים כלשהם).</span><span class="sxs-lookup"><span data-stu-id="e61b8-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="e61b8-108">**שלבים לפתרון בעיות בכניסה**</span><span class="sxs-lookup"><span data-stu-id="e61b8-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="e61b8-109">נווט אל דף הכניסה של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="e61b8-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="e61b8-110">הוסף כניסה למסנן לפי משתמש, טווח זמן, יישום, מצב, יישום לקוח וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="e61b8-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="e61b8-111">בחר אירוע כניסה והצג את הכרטיסיה ' גישה מותנית ' כדי לראות אילו פריטי מדיניות הוערכו.</span><span class="sxs-lookup"><span data-stu-id="e61b8-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="e61b8-112">לחץ על השורה של מדיניות כדי להציג את פרטי המדיניות ולהבין מדוע היא הוחלה.</span><span class="sxs-lookup"><span data-stu-id="e61b8-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="e61b8-113">**כלים לפתרון בעיות במדיניות גישה מותנית**</span><span class="sxs-lookup"><span data-stu-id="e61b8-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="e61b8-114">מצב דוח בלבד מאפשר לך להעריך מדיניות מבלי להשפיע על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="e61b8-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="e61b8-115">כלי ' מה-אם ' מאפשר לך לדמות אירועי כניסה ולראות אילו פריטי מדיניות חלים.</span><span class="sxs-lookup"><span data-stu-id="e61b8-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="e61b8-116">התובנות והדוחות של חוברת העבודה מציגות השפעה בזמן אמת על כל מדיניות.</span><span class="sxs-lookup"><span data-stu-id="e61b8-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="e61b8-117">**מדיניות הגנה בסיסית**</span><span class="sxs-lookup"><span data-stu-id="e61b8-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="e61b8-118">מדיניות הגנה בסיסית לא אושרה.</span><span class="sxs-lookup"><span data-stu-id="e61b8-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="e61b8-119">הם אינם נאכפים עוד ויוסרו בקרוב מפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="e61b8-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="e61b8-120">אנו ממליצים לאפשר [ברירות מחדל של אבטחה](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="e61b8-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="e61b8-121">לקבלת מידע נוסף אודות גישה מותנית, ראה:</span><span class="sxs-lookup"><span data-stu-id="e61b8-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="e61b8-122">[שיטות עבודה מומלצות לגישה מותנית ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [תנאים בגישה](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 מותנית [פקדים בגישה](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 מותנית [מיקומים בגישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="e61b8-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
