---
title: יצירת משתמש
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569730"
---
# <a name="create-user"></a><span data-ttu-id="4b093-102">יצירת משתמש</span><span class="sxs-lookup"><span data-stu-id="4b093-102">Create user</span></span>

<span data-ttu-id="4b093-103">**הודעה:**</span><span class="sxs-lookup"><span data-stu-id="4b093-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="4b093-104">[פחת של תמיכת הכניסה של WebView מ- Google החל מ- 4 בינואר 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="4b093-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="4b093-105">בדוק אם האפליקציות שלך עשויות להיות מושפעות על-ידי [ביצוע ההנחיות של Google](https://go.microsoft.com/fwlink/?linkid=2157323) לגבי תאימות הבדיקה.</span><span class="sxs-lookup"><span data-stu-id="4b093-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="4b093-106">הקפד להשתמש ב- Webview של המערכת או בדפדפן המערכת בעת כניסה למשתמשים באמצעות חשבונות Google לצרכן.</span><span class="sxs-lookup"><span data-stu-id="4b093-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="4b093-107">לקבלת מידע נוסף, [ראה בעיות בכניסה ליישום באמצעות דפדפן Chrome בלבד](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="4b093-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="4b093-108">**איני יכול ליצור משתמש חדש במדריך הכתובות של Azure AD**</span><span class="sxs-lookup"><span data-stu-id="4b093-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="4b093-109">ודא שאתה מורשה ליצור משתמש רגיל חדש.</span><span class="sxs-lookup"><span data-stu-id="4b093-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="4b093-110">רק תפקיד מנהל המערכת הכללי או מנהל המשתמשים ב- Azure Active Directory (AD) יכול ליצור משתמש רגיל חדש.</span><span class="sxs-lookup"><span data-stu-id="4b093-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="4b093-111">אם אינך נמצא באחד מהתפקידים הללו, בקש ממנהל מערכת להוסיף אותך לאחד התפקידים הללו או ליצור את חשבון המשתמש החדש בשבילך.</span><span class="sxs-lookup"><span data-stu-id="4b093-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="4b093-112">ודא לשם המשתמש נמצא בתחום שאומת ב- Azure AD שלך.</span><span class="sxs-lookup"><span data-stu-id="4b093-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="4b093-113">אם אין לך שמות תחומים מותאמים אישית מאומתים ב- Azure AD, באפשרותך להשתמש בתחום ההתחלתי של Azure AD, המסתיים ב- \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="4b093-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="4b093-114">ודא משם המשתמש נמצא בתחום שלא מאוחד ל- Azure AD מה- AD המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="4b093-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="4b093-115">לא ניתן להוסיף משתמשים בענן עם שמות תחומים מאוחדים מהסביבה המקומית.</span><span class="sxs-lookup"><span data-stu-id="4b093-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="4b093-116">ודא שלא קיים כבר שם משתמש או איש קשר אחר שברצונך להקצות למשתמש החדש.</span><span class="sxs-lookup"><span data-stu-id="4b093-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="4b093-117">שמות משתמשים חייבים להיות ייחודיים ברחבי Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4b093-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="4b093-118">ראה [תפקידים ומנהלי מערכת של Azure AD עבור](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4b093-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="4b093-119">ראה את [שמות התחומים עבור](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD שלך.</span><span class="sxs-lookup"><span data-stu-id="4b093-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="4b093-120">סקור [יומני ביקורת](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) כדי לראות מידע מפורט יותר אודות משתמש שנוצר לאחרונה או נמחק, כמו מי ביצע את הפעולה ומתי.</span><span class="sxs-lookup"><span data-stu-id="4b093-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="4b093-121">לקבלת מידע נוסף אודות הוספת משתמשים חדשים, ראה [שימוש בפורטל Azure כדי ליצור משתמש חדש ב- Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="4b093-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="4b093-122">[תפקידי ניהול של Azure AD](/azure/active-directory/active-directory-assign-admin-roles): הרשאות תפקיד מנהל מערכת ב- Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4b093-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="4b093-123">באפשרותך גם להשתמש [ב- Azure AD PowerShell כדי ליצור משתמש חדש.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="4b093-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
