---
title: בעיה באיפוס סיסמה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694376"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="828d8-102">בעיות באיפוס סיסמה</span><span class="sxs-lookup"><span data-stu-id="828d8-102">Problems resetting password</span></span>

<span data-ttu-id="828d8-103">להלן כמה מהבעיות שאתה עשוי לעמוד בהן בעת איפוס סיסמה ופתרונות אפשריים:</span><span class="sxs-lookup"><span data-stu-id="828d8-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="828d8-104">**אני נתקל בבעיה עם איפוס סיסמה שאינו מכוסה בקטגוריות האחרות**</span><span class="sxs-lookup"><span data-stu-id="828d8-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="828d8-105">ודא שאתה מורשה לאפס סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="828d8-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="828d8-106">רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.</span><span class="sxs-lookup"><span data-stu-id="828d8-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="828d8-107">מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.</span><span class="sxs-lookup"><span data-stu-id="828d8-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="828d8-108">ודא שהבנת את דרישות הרישוי:</span><span class="sxs-lookup"><span data-stu-id="828d8-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="828d8-109">דרוש לך רשיון אחד לפחות שהוקצה בארגון שלך</span><span class="sxs-lookup"><span data-stu-id="828d8-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="828d8-110">משתמשים בענן בלבד-כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic</span><span class="sxs-lookup"><span data-stu-id="828d8-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="828d8-111">משתמשים בענן ו/או מקומיים-תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)</span><span class="sxs-lookup"><span data-stu-id="828d8-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="828d8-112">לקבלת מידע נוסף אודות דרישות הרישוי, ראה [דרישות רישוי מאמר עבור איפוס סיסמה בשירות עצמי של תכלת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="828d8-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="828d8-113">**אני נתקל בבעיות בבדיקת מדיניות איפוס הסיסמה שהגדרתי**</span><span class="sxs-lookup"><span data-stu-id="828d8-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="828d8-114">מדיניות שהוחלו לאחרונה עשויה להימשך כמה דקות כדי לשכפל את כל מרכזי הנתונים ואת נקודות הקצה.</span><span class="sxs-lookup"><span data-stu-id="828d8-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="828d8-115">מרחק פיסי ממרכז הנתונים ישפיע גם על החלת השינויים במהירות.</span><span class="sxs-lookup"><span data-stu-id="828d8-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="828d8-116">בדיקה עם משתמש קצה, לא מנהל מערכת ופיילוט עם קבוצת משתמשים קטנה.</span><span class="sxs-lookup"><span data-stu-id="828d8-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="828d8-117">פריטי המדיניות המוגדרים בפורטל ' תכלת ' חלים רק על משתמשי קצה, לא על מנהלי מערכת.</span><span class="sxs-lookup"><span data-stu-id="828d8-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="828d8-118">Microsoft אוכפת מדיניות ברירת מחדל של איפוס סיסמה בשני שערים עבור כל תפקיד מנהל מערכת של תכלת (לדוגמה: מנהל מערכת כללי, מנהל מוקד התמיכה, מנהל הסיסמאות וכדומה)</span><span class="sxs-lookup"><span data-stu-id="828d8-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="828d8-119">קבל [מידע נוסף אודות פריטי מדיניות עבור מנהלי מערכת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="828d8-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="828d8-120">**ברצוני לפרוס איפוס סיסמה, אך איני מעוניין לגרום למשתמשים שלי לרשום מידע אבטחה נוסף**</span><span class="sxs-lookup"><span data-stu-id="828d8-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="828d8-121">אכלוס מראש של נתונים עבור המשתמשים שלך כדי שלא יצטרכו!</span><span class="sxs-lookup"><span data-stu-id="828d8-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="828d8-122">-כמנהל מערכת, באפשרותך להגדיר מאפייני טלפון ודואר אלקטרוני עבור המשתמשים שלך לפני שתפעיל את איפוס הסיסמה לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="828d8-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="828d8-123">באפשרותך לעשות זאת באמצעות התחברות ב-API, PowerShell או תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="828d8-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="828d8-124">מידע נוסף כאן:</span><span class="sxs-lookup"><span data-stu-id="828d8-124">More information here:</span></span>
- [<span data-ttu-id="828d8-125">פריסת איפוס סיסמה מבלי לחייב משתמשים לרשום</span><span class="sxs-lookup"><span data-stu-id="828d8-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="828d8-126">אילו נתונים משמשים לאיפוס סיסמה</span><span class="sxs-lookup"><span data-stu-id="828d8-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="828d8-127">**לחצן ' איפוס סיסמה ' מופיע באפור**</span><span class="sxs-lookup"><span data-stu-id="828d8-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="828d8-128">אין לך הרשאה לאפס את הסיסמאות של משתמש זה.</span><span class="sxs-lookup"><span data-stu-id="828d8-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="828d8-129">רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.</span><span class="sxs-lookup"><span data-stu-id="828d8-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="828d8-130">מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.</span><span class="sxs-lookup"><span data-stu-id="828d8-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="828d8-131">**איני רואה את להב איפוס הסיסמה**</span><span class="sxs-lookup"><span data-stu-id="828d8-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="828d8-132">אין לך הרשאה לאפס סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="828d8-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="828d8-133">רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.</span><span class="sxs-lookup"><span data-stu-id="828d8-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="828d8-134">מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.</span><span class="sxs-lookup"><span data-stu-id="828d8-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="828d8-135">**איני רואה את להב השילוב המקומי באיפוס סיסמה**</span><span class="sxs-lookup"><span data-stu-id="828d8-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="828d8-136">להב השילוב המקומי מופיע רק בסביבות היברידיות-כלומר, אתה משתמש ב-writeback password כדי לטפל בסיסמאות של משתמש מקומי.</span><span class="sxs-lookup"><span data-stu-id="828d8-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="828d8-137">אינך רואה את הלהב הזה אם:</span><span class="sxs-lookup"><span data-stu-id="828d8-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="828d8-138">אינך משתמש ב-password writeback</span><span class="sxs-lookup"><span data-stu-id="828d8-138">You are not using password writeback</span></span>
    - <span data-ttu-id="828d8-139">קיימת בעיה בהתקנה/בקישוריות של writeback סיסמה</span><span class="sxs-lookup"><span data-stu-id="828d8-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="828d8-140">קיימת בעיה בהתקנה/בקישוריות של התחברות של תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="828d8-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="828d8-141">לקבלת שלבים נוספים לפתרון בעיות עבור בעיות בwriteback סיסמאות, עיין בסעיף [פתרון בעיות בסיסמאות writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="828d8-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="828d8-142">**איני יודע כיצד לאפס סיסמת משתמש**</span><span class="sxs-lookup"><span data-stu-id="828d8-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="828d8-143">היכנס לפורטל ' תכלת ' כמנהל מתאים.</span><span class="sxs-lookup"><span data-stu-id="828d8-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="828d8-144">עבור אל הלהב משתמשים וקבוצות, בחר **את כל המשתמשים**.</span><span class="sxs-lookup"><span data-stu-id="828d8-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="828d8-145">בחר משתמש מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="828d8-145">Select a user from the list.</span></span>
1. <span data-ttu-id="828d8-146">עבור המשתמש שנבחר, בחר **מבט כולל** ולאחר מכן, בסרגל הפקודות, לחץ על **איפוס סיסמה**.</span><span class="sxs-lookup"><span data-stu-id="828d8-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="828d8-147">בצע את ההוראות המופיעות על המסך.</span><span class="sxs-lookup"><span data-stu-id="828d8-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="828d8-148">רק איפוסים שבוצעו באמצעות הסיסמה ' תמיכה בפורטל של writeback '.</span><span class="sxs-lookup"><span data-stu-id="828d8-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="828d8-149">**אני מאפס סיסמה של משתמש מקומי מפורטל הניהול של Office 365 או מהיישום Office 365 למכשירים ניידים, אך המשתמש עדיין אינו מצליח להיכנס**</span><span class="sxs-lookup"><span data-stu-id="828d8-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="828d8-150">Writeback סיסמה אינו נתמך בפורטל זה.</span><span class="sxs-lookup"><span data-stu-id="828d8-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="828d8-151">איפוס סיסמת המשתמש שוב בפורטל התכלת-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="828d8-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

