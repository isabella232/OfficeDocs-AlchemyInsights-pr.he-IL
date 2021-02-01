---
title: בעיות באישורים
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063630"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="25b00-102">בעיות באישורים</span><span class="sxs-lookup"><span data-stu-id="25b00-102">Issues with credentials</span></span>

<span data-ttu-id="25b00-103">[פלטפורמת הזהויות של Microsoft וזרימת אישורי הלקוח של OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) מתארת כיצד לתכנת ישירות מול אישורי הלקוח של OAuth 2.0 מעניקים זרימה.</span><span class="sxs-lookup"><span data-stu-id="25b00-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="25b00-104">**כיצד ניתן לנהל את הסיסמה או אישורי האישור של היישום?**</span><span class="sxs-lookup"><span data-stu-id="25b00-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="25b00-105">ב-תכלת CLI, באפשרותך להשתמש [באישור האפליקציה az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) כדי למחוק, לפרט או לאפס את הסיסמה או אישורי האישור של היישום.</span><span class="sxs-lookup"><span data-stu-id="25b00-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="25b00-106">**כיצד המשתמשים שלי מאפסים את הסיסמאות שלהם?**</span><span class="sxs-lookup"><span data-stu-id="25b00-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="25b00-107">המשתמשים צריכים [להירשם לאיפוס סיסמה בשירות עצמי](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) לפני שיוכלו לאפס את הסיסמאות שלהם.</span><span class="sxs-lookup"><span data-stu-id="25b00-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="25b00-108">לאחר שמשתמש נרשם, הם יכולים לבצע את ההוראות במאמר זה כדי לאפס את הסיסמה שלו: [לאפס את הסיסמה שלך בעבודה או בבית הספר](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="25b00-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="25b00-109">**כיצד המשתמשים שלי משנים את הסיסמאות שלהם?**</span><span class="sxs-lookup"><span data-stu-id="25b00-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="25b00-110">המשתמשים יכולים לבצע את השלבים המפורטים במאמר זה כדי לשנות את הסיסמאות שלהם: [כיצד לשנות את הסיסמה שלך](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="25b00-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="25b00-111">הם יכולים גם [לנהל סיסמאות של יישומים עבור אימות של שני שלבים](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="25b00-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="25b00-112">**המשתמש שלי מקבל שגיאה בעת שינוי או איפוס של הסיסמה שלו**</span><span class="sxs-lookup"><span data-stu-id="25b00-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="25b00-113">קישור זה יספק מידע על בעיות נפוצות שעלולות להתעורר כאשר משתמש מנסה לאפס את הסיסמה שלו: [בעיות נפוצות והפתרונות שלהם](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="25b00-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="25b00-114">**אני נתקל בבעיה באיפוס סיסמת משתמש**</span><span class="sxs-lookup"><span data-stu-id="25b00-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="25b00-115">ודא שאתה מורשה לאפס סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="25b00-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="25b00-116">*רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.*</span><span class="sxs-lookup"><span data-stu-id="25b00-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="25b00-117">מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.</span><span class="sxs-lookup"><span data-stu-id="25b00-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="25b00-118">ודא שהבנת את דרישות הרישוי:</span><span class="sxs-lookup"><span data-stu-id="25b00-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="25b00-119">דרוש לך רשיון אחד לפחות שהוקצה בארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="25b00-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="25b00-120">**משתמשים בענן בלבד** -כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic</span><span class="sxs-lookup"><span data-stu-id="25b00-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="25b00-121">**משתמשים בענן ו/או מקומיים** -תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)</span><span class="sxs-lookup"><span data-stu-id="25b00-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="25b00-122">לקבלת מידע נוסף על דרישות הרישוי, ראה [דרישות רישוי עבור איפוס סיסמה בשירות עצמי של תכלת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="25b00-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="25b00-123">כדי לאפס סיסמת משתמש, אתר את המשתמש בתכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="25b00-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="25b00-124">לאחר מכן, בלהב מבט כולל עבור משתמש זה, לחץ על לחצן ' איפוס סיסמה '.</span><span class="sxs-lookup"><span data-stu-id="25b00-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="25b00-125">**לחצן ' איפוס סיסמה ' מופיע באפור**</span><span class="sxs-lookup"><span data-stu-id="25b00-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="25b00-126">אין לך הרשאה לאפס את הסיסמאות של משתמש **זה** .</span><span class="sxs-lookup"><span data-stu-id="25b00-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="25b00-127">*רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.*</span><span class="sxs-lookup"><span data-stu-id="25b00-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="25b00-128">מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.</span><span class="sxs-lookup"><span data-stu-id="25b00-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="25b00-129">**איני רואה את להב איפוס הסיסמה**</span><span class="sxs-lookup"><span data-stu-id="25b00-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="25b00-130">אין לך הרשאה לאפס סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="25b00-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="25b00-131">*רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים.*</span><span class="sxs-lookup"><span data-stu-id="25b00-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="25b00-132">מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.</span><span class="sxs-lookup"><span data-stu-id="25b00-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="25b00-133">**איני רואה את להב השילוב המקומי באיפוס סיסמה**</span><span class="sxs-lookup"><span data-stu-id="25b00-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="25b00-134">להב השילוב המקומי מופיע רק בסביבות היברידיות-כלומר, אתה משתמש ב-writeback password כדי לטפל בסיסמאות של משתמש מקומי.</span><span class="sxs-lookup"><span data-stu-id="25b00-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="25b00-135">אינך רואה את הלהב הזה אם:</span><span class="sxs-lookup"><span data-stu-id="25b00-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="25b00-136">אינך משתמש ב-password writeback</span><span class="sxs-lookup"><span data-stu-id="25b00-136">You are not using password writeback</span></span>
  - <span data-ttu-id="25b00-137">קיימת בעיה בהתקנה/בקישוריות של writeback סיסמה</span><span class="sxs-lookup"><span data-stu-id="25b00-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="25b00-138">קיימת בעיה בהתקנה/בקישוריות של התחברות של תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="25b00-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="25b00-139">לקבלת שלבים נוספים לפתרון בעיות בנושא בעיות בwriteback סיסמאות, ראה [פתרון בעיות בסיסמאות writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="25b00-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="25b00-140">**איני יודע כיצד לאפס סיסמת משתמש**</span><span class="sxs-lookup"><span data-stu-id="25b00-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="25b00-141">היכנס לפורטל ' תכלת ' כמנהל מתאים.</span><span class="sxs-lookup"><span data-stu-id="25b00-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="25b00-142">עבור אל הלהב **משתמשים וקבוצות** , בחר **את כל המשתמשים**.</span><span class="sxs-lookup"><span data-stu-id="25b00-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="25b00-143">בחר משתמש מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="25b00-143">Select a user from the list.</span></span>
4. <span data-ttu-id="25b00-144">עבור המשתמש שנבחר, בחר **מבט כולל** ולאחר מכן, בסרגל הפקודות, בחר **איפוס סיסמה**.</span><span class="sxs-lookup"><span data-stu-id="25b00-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="25b00-145">בחר בלחצן **אפס סיסמה** ובצע את ההוראות המופיעות על המסך.</span><span class="sxs-lookup"><span data-stu-id="25b00-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="25b00-146">רק איפוסים שבוצעו באמצעות הסיסמה ' תמיכה **בפורטל** של writeback '.</span><span class="sxs-lookup"><span data-stu-id="25b00-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="25b00-147">**אני מאפס סיסמה של משתמש מקומי מפורטל הניהול של Office 365 או מהיישום Office 365 למכשירים ניידים, אך המשתמש עדיין אינו מצליח להיכנס**</span><span class="sxs-lookup"><span data-stu-id="25b00-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="25b00-148">Writeback סיסמה אינו נתמך בפורטל זה.</span><span class="sxs-lookup"><span data-stu-id="25b00-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="25b00-149">אפס את סיסמת המשתמש שוב בפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="25b00-149">Reset the user's password again in the Azure portal.</span></span>
