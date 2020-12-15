---
title: עדכן את כתובת המכירה והחיוב המשויכת לשלבים המומלצים שלך ב-MCA
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678476"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="02ab4-102">עדכן את כתובת המכירה והחיוב המשויכת לשלבים המומלצים שלך ב-MCA</span><span class="sxs-lookup"><span data-stu-id="02ab4-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="02ab4-103">באפשרותך לעדכן את כתובת המכירה והחיוב המשויכת להסכם הלקוחות של Microsoft (MCA).</span><span class="sxs-lookup"><span data-stu-id="02ab4-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="02ab4-104">רק מנהל מערכת יכול לבצע שינויים בפרטי פרופיל המשתמש של תכלת Active Directory.</span><span class="sxs-lookup"><span data-stu-id="02ab4-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="02ab4-105">אם לא הקצית את תפקיד מנהל המשתמש, פנה למנהל המשתמש שלך.</span><span class="sxs-lookup"><span data-stu-id="02ab4-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="02ab4-106">לקבלת מידע נוסף אודות שינוי פרופיל של משתמש, ראה [הוספה או עדכון של פרטי פרופיל של משתמש באמצעות ' תכלת Active Directory '](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="02ab4-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="02ab4-107">**כתובת מוכרת** -לכתובת הנמכרת היא הכתובת ופרטי הקשר של הארגון או האדם האחראי לחשבון חיוב.</span><span class="sxs-lookup"><span data-stu-id="02ab4-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="02ab4-108">הוא מוצג בכל החשבוניות שנוצרו עבור חשבון החיוב.</span><span class="sxs-lookup"><span data-stu-id="02ab4-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="02ab4-109">**כתובת לחיוב** -כתובת החיוב היא הכתובת ופרטי הקשר של הארגון או האדם האחראי על החשבוניות שנוצרו עבור חשבון חיוב.</span><span class="sxs-lookup"><span data-stu-id="02ab4-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="02ab4-110">עבור חשבון חיוב עבור MCA, יש כתובת לחיוב עבור כל פרופיל חיוב והוא מוצג בחשבונית שנוצרה עבור פרופיל החיוב.</span><span class="sxs-lookup"><span data-stu-id="02ab4-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="02ab4-111">**כדי לעדכן את הכתובת של חשבון חיוב של MCA**:</span><span class="sxs-lookup"><span data-stu-id="02ab4-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="02ab4-112">היכנס לפורטל התכלת באמצעות כתובת הדואר האלקטרוני, הכוללת בעלים או תפקיד משתתף בחשבון החיוב של MCA.</span><span class="sxs-lookup"><span data-stu-id="02ab4-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="02ab4-113">חפש חיוב של **ניהול עלויות**  +  .</span><span class="sxs-lookup"><span data-stu-id="02ab4-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="02ab4-114">לחץעל '  >  **עדכון מאפיינים ' נמכר**.</span><span class="sxs-lookup"><span data-stu-id="02ab4-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="02ab4-115">הזן את הכתובת החדשה ולחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="02ab4-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="02ab4-116">חשבונות מסוימים דורשים אימות נוסף לפני שניתן לעדכן את כתובתו הנמכרת.</span><span class="sxs-lookup"><span data-stu-id="02ab4-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="02ab4-117">אם החשבון שלך דורש אישור ידני, תתבקש לפנות לתמיכה בתכלת.</span><span class="sxs-lookup"><span data-stu-id="02ab4-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="02ab4-118">**כדי לעדכן כתובת של חשבון חיוב של MCA**:</span><span class="sxs-lookup"><span data-stu-id="02ab4-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="02ab4-119">היכנס לפורטל התכלת באמצעות כתובת הדואר האלקטרוני, הכוללת בעלים או תפקיד משתתף בחשבון חיוב או פרופיל חיוב עבור MCA.</span><span class="sxs-lookup"><span data-stu-id="02ab4-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="02ab4-120">חפש חיוב של **ניהול עלויות**  +  .</span><span class="sxs-lookup"><span data-stu-id="02ab4-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="02ab4-121">לחץ על **פרופילי חיוב** ובחר באפשרות בחר פרופיל חיוב כדי לעדכן את כתובת החיוב.</span><span class="sxs-lookup"><span data-stu-id="02ab4-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="02ab4-122">לחץ על  >  **כתובת עדכון** מאפיינים.</span><span class="sxs-lookup"><span data-stu-id="02ab4-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="02ab4-123">הזן את הכתובת החדשה ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="02ab4-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="02ab4-124">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="02ab4-124">**Recommended documents**</span></span>

<span data-ttu-id="02ab4-125">[שינוי פרטי קשר עבור חשבון חיוב של תכלת](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="02ab4-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="02ab4-126">עדכון הגדרות של חשבון חיוב</span><span class="sxs-lookup"><span data-stu-id="02ab4-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="02ab4-127">הכרת תפקידי ניהול של הסכם לקוח של Microsoft בתכלת</span><span class="sxs-lookup"><span data-stu-id="02ab4-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)