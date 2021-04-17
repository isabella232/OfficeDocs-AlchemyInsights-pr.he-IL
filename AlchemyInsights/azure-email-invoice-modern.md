---
title: הפקת חשבוניות דואר אלקטרוני מודרניות של Modern Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820827"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="cc3a9-102">הפקת חשבונית דואר אלקטרוני ב- Azure</span><span class="sxs-lookup"><span data-stu-id="cc3a9-102">Email invoicing in Azure</span></span>

<span data-ttu-id="cc3a9-103">כדי לעדכן את העדפת החשבונית של הדואר האלקטרוני, עליך להיות בעלים או בתפקיד משתתף בפרופיל החיוב או בחשבון החיוב.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="cc3a9-104">לאחר הבעת הסכמה להצטרפות, כל המשתמשים בעלי התפקידים, המשתתפים, הקוראים ומנהל החשבונית בפרופיל החיוב יקבלו את החשבונית בהודעת דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="cc3a9-105">היכנס לפורטל [פורטל Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cc3a9-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="cc3a9-106">חפש **ניהול עלויות + חיוב**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="cc3a9-107">בחר **חשבוניות** מימין ולאחר מכן בחר **חשבונית בדואר אלקטרוני** בחלק העליון של הדף.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="cc3a9-108">אם יש לך כמה פרופילי חיוב, בחר פרופיל חיוב ולאחר מכן בחר באפשרות **הצטרפות**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="cc3a9-109">בחר **עדכון**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-109">Select **Update**.</span></span>
6. <span data-ttu-id="cc3a9-110">אם יש לך כמה פרופילי חיוב, בחר פרופיל חיוב ולאחר מכן בחר באפשרות **הצטרפות**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="cc3a9-111">אתה נותן לאחרים גישה לצפות בחשבוניות, להוריד אותן ולשלם עבורן על-ידי הקצאתן לתפקיד מנהל החשבונית עבור פרופיל חיוב של MCA או MPA.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="cc3a9-112">אם בחרת לקבל את החשבונית בדואר אלקטרוני, גם המשתמשים יקבלו את החשבוניות בדואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="cc3a9-113">היכנס לפורטל [פורטל Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cc3a9-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="cc3a9-114">חפש **ניהול עלויות + חיוב**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="cc3a9-115">בחר **פרופילי חיוב** בצד ימין.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="cc3a9-116">מתוך רשימת פרופילי החיוב, בחר פרופיל חיוב שעבורו אתה מעוניין להקצות תפקיד מנהל חשבונית.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="cc3a9-117">בחר **בקרת גישה (IAM)** בצד ימין ולאחר מכן בחר **הוספה** בחלק העליון של הדף.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="cc3a9-118">ברשימת התפקידים הנפתחת, בחר **מנהל חשבוניות**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="cc3a9-119">למתן גישה, הזן את כתובת הדוא"ל של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="cc3a9-120">להקצאת התפקיד, בחר **שמירה**.</span><span class="sxs-lookup"><span data-stu-id="cc3a9-120">Select **Save** to assign the role.</span></span>
