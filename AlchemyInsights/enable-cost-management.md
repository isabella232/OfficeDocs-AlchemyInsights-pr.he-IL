---
title: הפיכת ניהול עלויות לזמין
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677736"
---
# <a name="enable-cost-management"></a><span data-ttu-id="6fb2a-102">הפיכת ניהול עלויות לזמין</span><span class="sxs-lookup"><span data-stu-id="6fb2a-102">Enable cost management</span></span>

<span data-ttu-id="6fb2a-103">**מה המשמעות של ' עלויות ' אינה זמינה עבור הארגון שלך?**</span><span class="sxs-lookup"><span data-stu-id="6fb2a-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="6fb2a-104">ארגונים המשתמשים בהסכם הארגון (EA) או בחשבונות Microsoft Customer (MCA) יכולים להפוך את הגישה למידע אודות עלויות ולמידע אודות תמחור ללא זמינה.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="6fb2a-105">לאחר כניסה לפורטל התכלת, הם יכולים להשתמש בממשקי ה-Api של החיוב כדי לקבל חשבוניות באופן תוכניתי (לאחר התחייבות) ופרטי שימוש.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="6fb2a-106">**כיצד לאפשר למשתמשים נוספים לגשת לחשבוניות**</span><span class="sxs-lookup"><span data-stu-id="6fb2a-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="6fb2a-107">עבור אל ' **להב מנויים** ' בפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="6fb2a-108">בחר **חשבוניות** ולאחר מכן **גש לחשבוניות**.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="6fb2a-109">הפעל את access ולאחר מכן שמור את השינויים, כדי לאפשר למשתמשים בתפקידים הנמצאים בטווח המנוי להוריד חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="6fb2a-110">מנהל החשבון יכול גם לקבוע תצורה של חשבוניות שנשלחות באמצעות דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="6fb2a-111">לקבלת מידע נוסף, ראה [קבלת החשבונית שלך בדואר אלקטרוני](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="6fb2a-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="6fb2a-112">**כיצד להוסיף משתמשים לתפקיד קורא החיובים**</span><span class="sxs-lookup"><span data-stu-id="6fb2a-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="6fb2a-113">עבור אל ' **להב מנויים** ' בפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="6fb2a-114">בחר **בקרת גישה (יאם)** ולאחר מכן לחץ על **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="6fb2a-115">בחר **קורא חיובים** בדף **' בחר תפקיד** '.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="6fb2a-116">הקלד את הודעת הדואר האלקטרוני של המשתמש שברצונך להזמין ולאחר מכן לחץ על **אישור** כדי לשלוח את ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="6fb2a-117">בצע את ההוראות המופיעות בהודעת הדואר האלקטרוני הזמנה כדי להיכנס כקורא חיוב.</span><span class="sxs-lookup"><span data-stu-id="6fb2a-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="6fb2a-118">לקבלת מידע נוסף, ראה [הענקת גישה לחיוב](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="6fb2a-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="6fb2a-119">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="6fb2a-119">**Recommended documents**</span></span>

- [<span data-ttu-id="6fb2a-120">הפיכת תצוגות של DA ו-AO לזמינות באמצעות פורטל EA</span><span class="sxs-lookup"><span data-stu-id="6fb2a-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="6fb2a-121">עלויות הכלולות בניהול עלויות</span><span class="sxs-lookup"><span data-stu-id="6fb2a-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="6fb2a-122">תמיכה ב-Microsoft תכולים מציעה</span><span class="sxs-lookup"><span data-stu-id="6fb2a-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="6fb2a-123">סקירת עלויות בניתוח עלות</span><span class="sxs-lookup"><span data-stu-id="6fb2a-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="6fb2a-124">מתן גישה לפרטי חיוב</span><span class="sxs-lookup"><span data-stu-id="6fb2a-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="6fb2a-125">בדיקת גישה להסכם לקוח של Microsoft</span><span class="sxs-lookup"><span data-stu-id="6fb2a-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






