---
title: בעיות בשימוש במסוף הניהול של Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555382"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="41301-102">בעיות בשימוש במסוף הניהול של Intune</span><span class="sxs-lookup"><span data-stu-id="41301-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="41301-103">**"הגישה נדחתה" בעת ניווט בפורטל הניהול של Intune.**</span><span class="sxs-lookup"><span data-stu-id="41301-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="41301-104">אם אתה חבר בתפקיד מותאם אישית Intune, ודא שרשיון של Intune או ' חבילת ניידות ארגונית ' (EMS) מוקצה לחשבונך.</span><span class="sxs-lookup"><span data-stu-id="41301-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="41301-105">אם אתה משתמש ב'מנהל התצורה ' כדי לנהל התקנים, ודא שאינך חלק מאוסף המשתמשים Intune עבור מנהל התצורה MDM.</span><span class="sxs-lookup"><span data-stu-id="41301-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="41301-106">ודא שהוקצתה לך הרשאות בקרת ניהול מבוססת תפקידים (RBAC) המתאימות בלהב התפקידים Intune.</span><span class="sxs-lookup"><span data-stu-id="41301-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="41301-107">ודא שהקבוצה שבשימוש אינה רשימת תפוצה.</span><span class="sxs-lookup"><span data-stu-id="41301-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="41301-108">Intune בפורטל התכלת תומך רק בחשבונות משתמשים השייכים לקבוצות האבטחה של הפעילות התכלת של הספרייה.</span><span class="sxs-lookup"><span data-stu-id="41301-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="41301-109">סקור את הקבוצות שלך בפורטל התכלת **הIntune**  >  **קבוצות**, או בפורטל **הפעיל של הספרייה הפעילה**.</span><span class="sxs-lookup"><span data-stu-id="41301-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="41301-110">**למשתמש יש הרשאות רבות מדי עבור תפקיד Intune שהוקצה**</span><span class="sxs-lookup"><span data-stu-id="41301-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="41301-111">ייעץ למשתמש לעבור אל **Intune**  >  **Intune תפקידים**  >  **שההרשאות שלי**  >  **מייצאים** כדי לסקור הרשאות מוענקות.</span><span class="sxs-lookup"><span data-stu-id="41301-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="41301-112">**הוספתי קבוצת טווחים לתפקיד, אך משתמשים באותו תפקיד עדיין יראו משתמשים או התקנים אחרים.**</span><span class="sxs-lookup"><span data-stu-id="41301-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="41301-113">קבוצות טווחים אינן מסננות משתמשים או התקנים.</span><span class="sxs-lookup"><span data-stu-id="41301-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="41301-114">קבוצות טווחים:</span><span class="sxs-lookup"><span data-stu-id="41301-114">Scope groups:</span></span>

- <span data-ttu-id="41301-115">הגבלה למי משתמשים יכולים להקצות מדיניות או יישומים.</span><span class="sxs-lookup"><span data-stu-id="41301-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="41301-116">אפשר למשתמשים מסוימים בלבד להפעיל משימות מרוחקות בהתקנים.</span><span class="sxs-lookup"><span data-stu-id="41301-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="41301-117">לקבלת מידע נוסף אודות קבוצות היקף, ראה [בקרת גישה מבוססת תפקידים (RBAC) עם Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="41301-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="41301-118">**הוספתי משתמש לתפקיד Intune אך עדיין יש להם גישה מלאה למסוף הניהול של Intune.**</span><span class="sxs-lookup"><span data-stu-id="41301-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="41301-119">נווט אל Intune > **משתמשים** בפורטל התכלת וודא שהמשתמש אינו מוקצה לאף אחד מהתפקידים הבאים בפורטל התכלת:</span><span class="sxs-lookup"><span data-stu-id="41301-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="41301-120">מנהל מערכת כללי</span><span class="sxs-lookup"><span data-stu-id="41301-120">Global administrator</span></span>
- <span data-ttu-id="41301-121">מנהל שירות Intune</span><span class="sxs-lookup"><span data-stu-id="41301-121">Intune service administrator</span></span>
- <span data-ttu-id="41301-122">מנהל מערכת של SharePoint</span><span class="sxs-lookup"><span data-stu-id="41301-122">SharePoint administrator</span></span>

<span data-ttu-id="41301-123">לקבלת מידע נוסף, ראה [בקרת גישה מבוססת תפקידים (RBAC) עם Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="41301-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="41301-124">**בעיות גישה**</span><span class="sxs-lookup"><span data-stu-id="41301-124">**Access Issues**</span></span>

<span data-ttu-id="41301-125">לקבלת מידע נוסף, ראה [אינך יכול להיכנס ל-Office 365, תכלת או Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="41301-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>