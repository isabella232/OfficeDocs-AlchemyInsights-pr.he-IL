---
title: פתרון בעיות ב-SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429719"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="3d735-102">פתרון בעיות ב-SSPR</span><span class="sxs-lookup"><span data-stu-id="3d735-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="3d735-103">**אני נתקל בבעיות בקביעת התצורה של איפוס סיסמה**</span><span class="sxs-lookup"><span data-stu-id="3d735-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="3d735-104">אם אתה מנהל מערכת ומחפש כיצד להפוך איפוס סיסמה בשירות עצמי לזמין, ראה [ערכת לימוד הפעלת SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), כדי לקבוע את התצורה של איפוס סיסמה עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="3d735-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="3d735-105">ייתכן שתרצה גם לסקור את [דרישות הרישוי](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3d735-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="3d735-106">דרוש לך רשיון אחד לפחות המוקצה לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="3d735-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="3d735-107">**משתמשים בענן בלבד** -כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic</span><span class="sxs-lookup"><span data-stu-id="3d735-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="3d735-108">**משתמשים בענן ו/או מקומיים** -תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)</span><span class="sxs-lookup"><span data-stu-id="3d735-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="3d735-109">לקבלת שאלות נוספות אודות איפוס סיסמה בשירות עצמי, עיין בשאלות [הנפוצות שלנו](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3d735-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3d735-110">**אני מקבל הודעת שגיאה**</span><span class="sxs-lookup"><span data-stu-id="3d735-110">**I'm getting an error message**</span></span>

<span data-ttu-id="3d735-111">עיין במאמר זה כדי לאתר שגיאות נפוצות והפתרונות שלהן: [פתרון בעיות באיפוס סיסמה בשירות עצמי](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="3d735-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="3d735-112">**אני נתקל בבעיה במדיניות ' איפוס הסיסמה שלי '**</span><span class="sxs-lookup"><span data-stu-id="3d735-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="3d735-113">אם מדיניות איפוס הסיסמאות אינה מתנהגת כמצופה, או אם יש לך שאלות לגבי מדיניות איפוס סיסמה, עיין [במאמר זה: מדיניות סיסמה והגבלות ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3d735-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="3d735-114">מדיניות איפוס סיסמאות אינה חלה על מנהלי מערכת.</span><span class="sxs-lookup"><span data-stu-id="3d735-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="3d735-115">Microsoft אוכפת מדיניות ברירת מחדל מסוג ברירת מחדל לאיפוס סיסמה עבור כל תפקיד מנהל מערכת של תכלת.</span><span class="sxs-lookup"><span data-stu-id="3d735-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="3d735-116">ודא שאתה בוחן עם משתמש שאינו מנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="3d735-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="3d735-117">לקבלת מידע נוסף אודות מדיניות איפוס מנהל מערכת, עיין במאמר זה: [איפוס הבדלי מדיניות של מנהל מערכת](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="3d735-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="3d735-118">**איני מעוניין שהמשתמשים יוכלו לרשום פרטי אבטחה נוספים עבור איפוס סיסמה**</span><span class="sxs-lookup"><span data-stu-id="3d735-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="3d735-119">באפשרותך לאכלס מראש נתונים (דואר אלקטרוני ותכונות טלפון) עבור המשתמשים שלך באמצעות מחבר API, PowerShell או תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="3d735-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="3d735-120">כדי ללמוד כיצד לקרוא:</span><span class="sxs-lookup"><span data-stu-id="3d735-120">To learn how read:</span></span>

- [<span data-ttu-id="3d735-121">פריסת איפוס סיסמה מבלי לחייב משתמשים לרשום</span><span class="sxs-lookup"><span data-stu-id="3d735-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="3d735-122">אילו נתונים משמשים לאיפוס סיסמה</span><span class="sxs-lookup"><span data-stu-id="3d735-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3d735-123">**אני מעוניין שהמשתמשים שלי ירשמו את פרטי האבטחה הנוספים שלהם לאיפוס סיסמה**</span><span class="sxs-lookup"><span data-stu-id="3d735-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="3d735-124">בקש מהמשתמשים לרשום את מידע האבטחה שלהם עבור איפוס סיסמה בשירות עצמי על-ידי הפניית הקישור אל [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="3d735-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="3d735-125">לאחר שהנתונים מאוכלסים עבור המשתמש (על-ידי המשתמש או על-ידי מנהל המערכת), הפנה את המשתמש שלך ל- [aka.ms/sspr](https://passwordreset.microsoftonline.com/) כדי שהמשתמשים יוכלו להיות מוסמכים כדי לאפס את הסיסמאות שלהם.</span><span class="sxs-lookup"><span data-stu-id="3d735-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="3d735-126">אם המשתמשים עדיין חווים בעיות, הם ככל הנראה משתמשים מסונכרנים ב-hash **מאוחדים** או **בסיסמאות** .</span><span class="sxs-lookup"><span data-stu-id="3d735-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="3d735-127">משמעות הדבר היא שסביר להניח שקיימת בעיה בשירות Password Writeback.</span><span class="sxs-lookup"><span data-stu-id="3d735-127">This means there is likely a problem with the Password Writeback service.</span></span>