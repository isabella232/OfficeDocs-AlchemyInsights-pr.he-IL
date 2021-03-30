---
title: יישום אימות
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405062"
---
# <a name="authentication-app"></a><span data-ttu-id="f0314-102">יישום אימות</span><span class="sxs-lookup"><span data-stu-id="f0314-102">Authentication app</span></span>

<span data-ttu-id="f0314-103">אם אתה מנהל מערכת כללי, תוכל לגלות במהירות מה קרה או לאבחן בעיות הקשורות להכניסה של המשתמש באמצעות אבחון [הכניסה.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="f0314-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="f0314-104">הפעל את האבחון על-ידי לחיצה על לחצן "[הפעל אבחון](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)".</span><span class="sxs-lookup"><span data-stu-id="f0314-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="f0314-105">אתר את האירוע שיש לנתח על-ידי הזנת הפרטים שיש לך לגבי המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.</span><span class="sxs-lookup"><span data-stu-id="f0314-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="f0314-106">סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואת הפעולות שתוכל לבצע כדי לבצע שינויים, אם יש צורך בשינויים.</span><span class="sxs-lookup"><span data-stu-id="f0314-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="f0314-107">**בדוק את התרחיש הרלוונטי:**</span><span class="sxs-lookup"><span data-stu-id="f0314-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="f0314-108">אם משתמש אינו מקבל הודעת דחיפה באפליקציית Microsoft Authenticator, ודא שהוא אינו מוצג תחת המשתמשים החסומים של MFA, כמתואר בחסימה [ובפיטורים של משתמשים.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="f0314-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="f0314-109">אם המשתמש אינו חסום עבור MFA אך אינו מקבל הודעת דחיפה, הוא יכול לפתוח את האפליקציה Microsoft Authenticator, אשר תמשוך את בקשות האישור הממתינות.</span><span class="sxs-lookup"><span data-stu-id="f0314-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="f0314-110">כשיטת כניסה חלופית, המשתמש יכול גם ללחוץ על היכנס בדרך אחרת ולבחור להשתמש בקוד אימות מהאפליקציה למכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="f0314-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="f0314-111">אפליקציית Microsoft Authenticator היא השיטה הזמינה היחידה עבור משתמשים רבים.</span><span class="sxs-lookup"><span data-stu-id="f0314-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="f0314-112">[קבל מידע נוסף על ברירות מחדל של](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)אבטחה , עיין בשאלות הנפוצות בנושא אפליקציית [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) לקבלת שאלות נפוצות ואופן פתרון אותן.</span><span class="sxs-lookup"><span data-stu-id="f0314-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="f0314-113">**סרטוני וידאו מומלצים**</span><span class="sxs-lookup"><span data-stu-id="f0314-113">**Recommended Videos**</span></span>

<span data-ttu-id="f0314-114">[כיצד להגדיר יישום Authenticator בטלפון חדש (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f0314-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
