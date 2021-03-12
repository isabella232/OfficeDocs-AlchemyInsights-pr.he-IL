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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744974"
---
# <a name="create-user"></a><span data-ttu-id="d826f-102">יצירת משתמש</span><span class="sxs-lookup"><span data-stu-id="d826f-102">Create user</span></span>

<span data-ttu-id="d826f-103">**ודעה**</span><span class="sxs-lookup"><span data-stu-id="d826f-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="d826f-104">[תבטלות של תמיכה בכניסה של תצוגת האינטרנט מ-Google החל מ-4 בינואר 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span><span class="sxs-lookup"><span data-stu-id="d826f-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="d826f-105">בדיקה אם היישומים שלך עשויים להיות מושפעים על-ידי ביצוע [ההדרכה של Google](https://go.microsoft.com/fwlink/?linkid=2157323) לגבי תאימות בדיקות.</span><span class="sxs-lookup"><span data-stu-id="d826f-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="d826f-106">הקפד להשתמש בתצוגת האינטרנט של המערכת או בדפדפן המערכת בעת הכניסה למשתמשים שלך באמצעות חשבונות של Google לצרכן.</span><span class="sxs-lookup"><span data-stu-id="d826f-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="d826f-107">לקבלת מידע נוסף, ראה [בעיות בכניסה ליישומים באמצעות דפדפן Chrome בלבד](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="d826f-107">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="d826f-108">**איני מצליח ליצור משתמש חדש במדריך הכתובות של תכלת**</span><span class="sxs-lookup"><span data-stu-id="d826f-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="d826f-109">ודא שאתה מורשה ליצור משתמש רגיל חדש.</span><span class="sxs-lookup"><span data-stu-id="d826f-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="d826f-110">רק התפקיד ' מנהל מערכת כללי ' או ' מנהל משתמשים ' ב-תכלת Active Directory (AD) יכול ליצור משתמש רגיל חדש.</span><span class="sxs-lookup"><span data-stu-id="d826f-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="d826f-111">אם אינך נמצא באחד מתפקידים אלה, בקש ממנהל מערכת להוסיף אותך לאחד מתפקידים אלה או כדי ליצור את חשבון המשתמש החדש עבורך.</span><span class="sxs-lookup"><span data-stu-id="d826f-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="d826f-112">ודא ששם המשתמש נמצא בתחום שאומת במודעת התכלת.</span><span class="sxs-lookup"><span data-stu-id="d826f-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="d826f-113">אם אין לך שמות תחומים מותאמים אישית מאומתים במודעת התכלת שלך, באפשרותך להשתמש בתחום הראשוני של המודעה של תכלת, שמסתיים ב-\*. onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="d826f-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="d826f-114">ודא ששם המשתמש נמצא בתחום שאינו מאוחד לתכלת לספירה מהמודעה המקומית שלך.</span><span class="sxs-lookup"><span data-stu-id="d826f-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="d826f-115">לא ניתן להוסיף משתמשים בענן באמצעות שמות תחומים המאוחדים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="d826f-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="d826f-116">ודא שאין למשתמש או איש קשר אחר כבר את שם המשתמש שברצונך להקצות למשתמש החדש.</span><span class="sxs-lookup"><span data-stu-id="d826f-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="d826f-117">שמות משתמשים חייבים להיות ייחודיים בין תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="d826f-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="d826f-118">ראה [תפקידים ומנהלי מערכת של ' תכלת '](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) עבור הודעת התכלת.</span><span class="sxs-lookup"><span data-stu-id="d826f-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="d826f-119">ראה את [שמות התחומים](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) עבור הודעת התכלת.</span><span class="sxs-lookup"><span data-stu-id="d826f-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="d826f-120">סקור [יומני ביקורת](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) כדי לראות מידע מפורט יותר אודות משתמש שנוצר או נמחק לאחרונה, כגון מי שביצע את הפעולה ומתי.</span><span class="sxs-lookup"><span data-stu-id="d826f-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="d826f-121">לקבלת מידע נוסף אודות הוספת משתמשים חדשים, ראה [שימוש בפורטל ' תכלת ' כדי ליצור משתמש חדש במודעת התכלת](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d826f-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="d826f-122">[תפקידים מנהליים של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): הרשאות תפקיד מנהל מערכת ב-תכלת active Directory</span><span class="sxs-lookup"><span data-stu-id="d826f-122">[Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="d826f-123">[באפשרותך גם להשתמש ב-תכולים AD PowerShell כדי ליצור משתמש חדש](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span><span class="sxs-lookup"><span data-stu-id="d826f-123">You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
