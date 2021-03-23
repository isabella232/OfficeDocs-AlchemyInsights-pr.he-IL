---
title: בעיות בניהול משתמשים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036282"
---
# <a name="user-management-issues"></a><span data-ttu-id="a5fec-102">בעיות בניהול משתמשים</span><span class="sxs-lookup"><span data-stu-id="a5fec-102">User management issues</span></span>

<span data-ttu-id="a5fec-103">**מה קורה למשתמשים המוקצים הנוכחיים ליישום אם אני מבטל את המאפיין ' הקצאת משתמשים נדרשת ' (הגדר מאפיין זה ללא)?**</span><span class="sxs-lookup"><span data-stu-id="a5fec-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="a5fec-104">הפיכת **הקצאת משתמשים** ללא זמינה אינה משפיעה על המשתמשים המוקצים כעת.</span><span class="sxs-lookup"><span data-stu-id="a5fec-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="a5fec-105">הפיכת מאפיין זה ללא זמין יאפשר לכל המשתמשים לגשת ליישום.</span><span class="sxs-lookup"><span data-stu-id="a5fec-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="a5fec-106">כל המשתמשים הרשומים והמשתמשים שהוקצו לקבוצות ביישום עדיין יהיו חוקיים.</span><span class="sxs-lookup"><span data-stu-id="a5fec-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="a5fec-107">כדי להגביל את האפליקציה שלך לקבוצה ספציפית של משתמשים, ראה- [הגבל את האפליקציה ' לספירה לכיוון תכלת ' לקבוצת משתמשים-פלטפורמת הזהות של Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="a5fec-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="a5fec-108">כדי להקצות משתמשים וקבוצות, ליישומים ארגוניים ב-תכלת Active Directory (תכלת לספירה), מתוך הפורטל ' תכלת ' או באמצעות PowerShell, ראה [ניהול הקצאת משתמשים עבור יישום ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="a5fec-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="a5fec-109">כדי להקצות הרשאות ליצירה ולניהול יישומים, ראה [הקצאת הרשאות של מנהל מערכת לניהול יישומים-תכלת לספירה | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="a5fec-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="a5fec-110">**הסתרת יישומים ארגוניים ספציפיים ממשתמשים** -השתמש בשלבים הבאים כדי להסתיר את כל יישומי Microsoft 365 מהחלונית **היישומים שלי** .</span><span class="sxs-lookup"><span data-stu-id="a5fec-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="a5fec-111">היישומים עדיין יהיו גלויים בפורטל של Office 365.</span><span class="sxs-lookup"><span data-stu-id="a5fec-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="a5fec-112">היכנס לפורטל תכלת כמנהל מערכת כללי עבור מדריך הכתובות שלך.</span><span class="sxs-lookup"><span data-stu-id="a5fec-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="a5fec-113">בחר באפשרות **תכלת Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="a5fec-114">בחר **משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="a5fec-115">בחר **הגדרות משתמש**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="a5fec-116">תחת **יישומי Enterprise**, לחץ על **נהל את האופן שבו משתמשי הקצה מפעילים ומציגים את היישומים שלהם**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="a5fec-117">עבור **משתמשים יכולים לראות רק יישומי office 365 בפורטל של office 365**, לחץ על **כן**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="a5fec-118">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="a5fec-119">לקבלת פרטים נוספים, ראה [הסתרת יישום ארגוני מתוך חוויית המשתמש בתכלת לספירה | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="a5fec-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="a5fec-120">אם אתה מציע תוכנה כיישום שירות (SaaS) לארגונים רבים, באפשרותך לקבוע את התצורה של האפליקציה לקבל כניסה מכל הדיירים הפעילים של כתובות Active Directory (תכלת AD).</span><span class="sxs-lookup"><span data-stu-id="a5fec-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="a5fec-121">תצורה זו נקראת "ביצוע ריבוי דיירים ביישום שלך".</span><span class="sxs-lookup"><span data-stu-id="a5fec-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="a5fec-122">משתמשים בכל דייר המודע של תכלת יוכלו להיכנס לאפליקציה לאחר שתסכים להשתמש בחשבון שלו עם האפליקציה שלך.</span><span class="sxs-lookup"><span data-stu-id="a5fec-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="a5fec-123">לקבלת מידע נוסף, ראה [בניית יישומים החותמים על משתמשי הודעות תכלת-פלטפורמת הזהות של Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="a5fec-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="a5fec-124">**כיצד משתמש הקצה יכול לגשת לאפליקציה לאחר שהוא מוקצה ליישום?**</span><span class="sxs-lookup"><span data-stu-id="a5fec-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="a5fec-125">כל יישום בלהב יישום Enterprise מכיל קישור לגישה למשתמשי קצה.</span><span class="sxs-lookup"><span data-stu-id="a5fec-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="a5fec-126">משתמשים יכולים גם לגשת לאפליקציה דרך פורטל **היישומים שלי** בדרך קלה.</span><span class="sxs-lookup"><span data-stu-id="a5fec-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="a5fec-127">**רוצה לדעת אילו יישומים וסוג יישומים נמצאים בשימוש על-ידי משתמשים?**</span><span class="sxs-lookup"><span data-stu-id="a5fec-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="a5fec-128">באפשרותך להוריד דוחות כניסה עבור 30 הימים האחרונים מ- **portal.azure.com >-תכלת active directory> Signins> הורדת דוחות**.</span><span class="sxs-lookup"><span data-stu-id="a5fec-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="a5fec-129">למד כיצד [להעניק הסכמה של מנהל מערכת של דייר רחב ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) [ולקבוע את האופן שבו משתמשי קצה מתנגדים ליישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span><span class="sxs-lookup"><span data-stu-id="a5fec-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="a5fec-130">הכרת [אופן הפעולה של הסכמה](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [וניהול הסכמה ליישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span><span class="sxs-lookup"><span data-stu-id="a5fec-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


