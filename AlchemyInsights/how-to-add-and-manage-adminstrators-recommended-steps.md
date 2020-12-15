---
title: כיצד להוסיף ולנהל adminstrators-שלבים מומלצים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677803"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="2cf20-102">כיצד להוסיף ולנהל adminstrators-שלבים מומלצים</span><span class="sxs-lookup"><span data-stu-id="2cf20-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="2cf20-103">**עריכת מנהל המנוי או מנהל מערכת משותף**</span><span class="sxs-lookup"><span data-stu-id="2cf20-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="2cf20-104">מנהל החשבון יכול לערוך את שני התפקידים בעוד שמנהל המנוי יכול לשנות רק מנהלים משותפים [בפורטל התכלת](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="2cf20-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="2cf20-105">הוספה או שינוי של מנהלי מנויים של תכלת</span><span class="sxs-lookup"><span data-stu-id="2cf20-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="2cf20-106">**עדכון מנהל המנוי או Co-Administrator עבור מנויים פנימיים (משודרים)**</span><span class="sxs-lookup"><span data-stu-id="2cf20-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="2cf20-107">מנהל השירות או מנהל המערכת המשותף יכולים לשרת פעולה זו באופן עצמאי באמצעות השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2cf20-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="2cf20-108">היכנס [לפורטל תכלת](https://ms.portal.azure.com/#home) ולחץ על **ניהול עלות + חיוב** בלהב הימני.</span><span class="sxs-lookup"><span data-stu-id="2cf20-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="2cf20-109">לחץ על פריט השורה עם המנוי שלך.</span><span class="sxs-lookup"><span data-stu-id="2cf20-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="2cf20-110">פעולה זו פותחת את הסקירה עבור המנוי שלך.</span><span class="sxs-lookup"><span data-stu-id="2cf20-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="2cf20-111">בלהב **המנוי** , לחץ על **מאפיינים**.</span><span class="sxs-lookup"><span data-stu-id="2cf20-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="2cf20-112">לחץ על לחצן **מנהל השירות** .</span><span class="sxs-lookup"><span data-stu-id="2cf20-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="2cf20-113">הזן את הודעת הדואר האלקטרוני של המשתמש שברצונך להגדיר כמנהל שירות ולחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="2cf20-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="2cf20-114">**הוספה/שינוי/הסרה של מנהל מערכת משותף**</span><span class="sxs-lookup"><span data-stu-id="2cf20-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="2cf20-115">היכנס [לפורטל התכלת](https://ms.portal.azure.com/#home) כמנהל שירות.</span><span class="sxs-lookup"><span data-stu-id="2cf20-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="2cf20-116">פתח [מנויים](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ובחר מנוי.</span><span class="sxs-lookup"><span data-stu-id="2cf20-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="2cf20-117">(ניתן להקצות את adminstrators בטווח המנוי בלבד).</span><span class="sxs-lookup"><span data-stu-id="2cf20-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="2cf20-118">נווט אל   >  **מנהלי מערכת קלאסיים** של בקרת גישה (יאם)  >    >  הוסף **הוסף מנהל מערכת** כדי לפתוח את החלונית **הוספת מנהל משותף** (אם האפשרות הוסף מנהל משותף אינה זמינה, היא מציינת שאין לך הרשאות).</span><span class="sxs-lookup"><span data-stu-id="2cf20-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="2cf20-119">בחר את המשתמש שברצונך להוסיף ולחץ על **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="2cf20-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="2cf20-120">**למד עוד:**</span><span class="sxs-lookup"><span data-stu-id="2cf20-120">**Learn more:**</span></span>
- [<span data-ttu-id="2cf20-121">הוספת מנהל מערכת משותף</span><span class="sxs-lookup"><span data-stu-id="2cf20-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2cf20-122">הסרת מנהל מערכת משותף</span><span class="sxs-lookup"><span data-stu-id="2cf20-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2cf20-123">שינוי מנהל השירות</span><span class="sxs-lookup"><span data-stu-id="2cf20-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2cf20-124">הצגת מנהל החשבון</span><span class="sxs-lookup"><span data-stu-id="2cf20-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2cf20-125">ניהול גישה באמצעות הפורטל של RBAC ותכלת</span><span class="sxs-lookup"><span data-stu-id="2cf20-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="2cf20-126">**הוספה/מחיקה של משתמשים באמצעות ' תכלת Active Directory ' (AD)**</span><span class="sxs-lookup"><span data-stu-id="2cf20-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="2cf20-127">באפשרותך להוסיף משתמשים חדשים או למחוק משתמשים קיימים מארגון תכלת Active Directory (תכלת לספירה):</span><span class="sxs-lookup"><span data-stu-id="2cf20-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="2cf20-128">כדי להוסיף משתמש חדש, היכנס [לפורטל תכלת](https://ms.portal.azure.com/#home) כמנהל משתמש עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="2cf20-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="2cf20-129">בחר באפשרות **תכלת Active Directory**, בחר **משתמשים** ולאחר מכן לחץ על **משתמש חדש**.</span><span class="sxs-lookup"><span data-stu-id="2cf20-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="2cf20-130">בדף **המשתמש** , מלא את המידע הנדרש.</span><span class="sxs-lookup"><span data-stu-id="2cf20-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="2cf20-131">לחץ על **צור**.</span><span class="sxs-lookup"><span data-stu-id="2cf20-131">Click **Create**.</span></span> <span data-ttu-id="2cf20-132">המשתמש נוצר ונוסף לדייר המודע של תכלת.</span><span class="sxs-lookup"><span data-stu-id="2cf20-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="2cf20-133">**מידע נוסף**:</span><span class="sxs-lookup"><span data-stu-id="2cf20-133">**Learn more**:</span></span>

- [<span data-ttu-id="2cf20-134">הוספת משתמש חדש</span><span class="sxs-lookup"><span data-stu-id="2cf20-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="2cf20-135">מחיקת משתמש</span><span class="sxs-lookup"><span data-stu-id="2cf20-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="2cf20-136">הוספה או עדכון של פרטי פרופיל של משתמש באמצעות ' תכלת Active Directory '</span><span class="sxs-lookup"><span data-stu-id="2cf20-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="2cf20-137">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="2cf20-137">**Recommended documents**</span></span>

- [<span data-ttu-id="2cf20-138">מהו בקרת גישה מבוססת תפקידים (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="2cf20-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="2cf20-139">הבנת התפקידים השונים בתכלת</span><span class="sxs-lookup"><span data-stu-id="2cf20-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="2cf20-140">הרשאות תפקיד מנהל מערכת ב-תכלת Active Directory</span><span class="sxs-lookup"><span data-stu-id="2cf20-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="2cf20-141">ערכת לימוד: הענקת גישה למשתמש באמצעות RBAC ופורטל תכלת</span><span class="sxs-lookup"><span data-stu-id="2cf20-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="2cf20-142">פתרון בעיות ב-RBAC בתכלת</span><span class="sxs-lookup"><span data-stu-id="2cf20-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="2cf20-143">ארגון משאבים עם קבוצות ניהול של ' תכלת '</span><span class="sxs-lookup"><span data-stu-id="2cf20-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="2cf20-144">כיצד לבקש עותק של חשבונית התכלת באמצעות דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="2cf20-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="2cf20-145">כיצד להוסיף, לעדכן או להסיר כרטיס אשראי או חיוב מתכלת</span><span class="sxs-lookup"><span data-stu-id="2cf20-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="2cf20-146">ניהול (הפעלה מחדש של מנוי/ביטול/מעבר)</span><span class="sxs-lookup"><span data-stu-id="2cf20-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



