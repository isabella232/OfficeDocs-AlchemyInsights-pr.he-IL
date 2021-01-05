---
title: כיצד להוסיף ולנהל מנהלי מערכת
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755496"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="433a2-102">כיצד להוסיף ולנהל מנהלי מערכת</span><span class="sxs-lookup"><span data-stu-id="433a2-102">How to add and manage admins</span></span>

<span data-ttu-id="433a2-103">בהתבסס על תיאור הבעיה שלך, מצאנו פתרון עבורך.</span><span class="sxs-lookup"><span data-stu-id="433a2-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="433a2-104">רוב הלקוחות הצליחו לפתור את הבעיה שלהם בעצמם לאחר ביצוע התיעוד שלנו.</span><span class="sxs-lookup"><span data-stu-id="433a2-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="433a2-105">כדי לנהל את חשבון החיוב שלך עבור הסכם לקוח של Microsoft (MCA), באפשרותך להשתמש בתפקידים שונים עם רמת הגישה הרצויה.</span><span class="sxs-lookup"><span data-stu-id="433a2-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="433a2-106">תפקידים אלה מתקיימים בנוסף לתפקידי שירות התכלת המוכללים שעוזרים לך לשלוט במשאבים שלך.</span><span class="sxs-lookup"><span data-stu-id="433a2-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="433a2-107">**כדי להוסיף תפקידי חיוב בפורטל ' תכלת ':**</span><span class="sxs-lookup"><span data-stu-id="433a2-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="433a2-108">היכנס [לפורטל התכלת](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="433a2-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="433a2-109">חפש את *ניהול העלויות + חיוב*.</span><span class="sxs-lookup"><span data-stu-id="433a2-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="433a2-110">בחר בקרת גישה (יאם) בטווח כגון חשבון חיוב, פרופיל חיוב או מקטע חשבונית במקום שבו ברצונך להעניק גישה.</span><span class="sxs-lookup"><span data-stu-id="433a2-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="433a2-111">הדף בקרת גישה (יאם) מפרט משתמשים וקבוצות המוקצים לכל תפקיד עבור טווח זה.</span><span class="sxs-lookup"><span data-stu-id="433a2-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="433a2-112">כדי להעניק גישה למשתמש, בחר **הוסף** מראש הדף.</span><span class="sxs-lookup"><span data-stu-id="433a2-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="433a2-113">ברשימה הנפתחת *תפקיד* , בחר תפקיד.</span><span class="sxs-lookup"><span data-stu-id="433a2-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="433a2-114">הזן את כתובת הדואר האלקטרוני של המשתמש שאליו ברצונך להעניק גישה.</span><span class="sxs-lookup"><span data-stu-id="433a2-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="433a2-115">בחר **שמור** כדי להקצות את התפקיד.</span><span class="sxs-lookup"><span data-stu-id="433a2-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="433a2-116">כדי להסיר גישה עבור משתמש, בחר את המשתמש עם הקצאת התפקיד שברצונך להסיר.</span><span class="sxs-lookup"><span data-stu-id="433a2-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="433a2-117">בחר **הסר**.</span><span class="sxs-lookup"><span data-stu-id="433a2-117">Select **Remove**.</span></span>

<span data-ttu-id="433a2-118">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="433a2-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="433a2-119">הגדרות תפקיד חיוב</span><span class="sxs-lookup"><span data-stu-id="433a2-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="433a2-120">תפקידים ומשימות של חשבונות חיוב</span><span class="sxs-lookup"><span data-stu-id="433a2-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="433a2-121">תחילת העבודה עם חשבון החיוב שלך ב-MCA</span><span class="sxs-lookup"><span data-stu-id="433a2-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="433a2-122">בדיקת גישה להסכם לקוח של Microsoft</span><span class="sxs-lookup"><span data-stu-id="433a2-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
