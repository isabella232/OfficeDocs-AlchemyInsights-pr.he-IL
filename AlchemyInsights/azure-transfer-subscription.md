---
title: העבר את בעלות החיוב של תכלת
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922076"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="9cffd-102">העבר את בעלות החיוב של תכלת</span><span class="sxs-lookup"><span data-stu-id="9cffd-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="9cffd-103">היכנס [לפורטל התכלת](https://portal.azure.com/) כמנהל מערכת של חשבון החיוב המכיל את המנוי שברצונך להעביר.</span><span class="sxs-lookup"><span data-stu-id="9cffd-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="9cffd-104">אם אינך בטוח אם אתה מנהל מערכת, או אם עליך לקבוע מי כן, ראה [קביעת מנהל חיוב של חשבון](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="9cffd-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="9cffd-105">חיפוש **בניהול עלויות + חיוב**.</span><span class="sxs-lookup"><span data-stu-id="9cffd-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="9cffd-106">בחר **מנויים** מהחלונית הימנית.</span><span class="sxs-lookup"><span data-stu-id="9cffd-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="9cffd-107">בהתאם לגישה, ייתכן שיהיה עליך לבחור טווח חיוב ולאחר **מכן להיכנס** למנויים או **למנויי תכלת**.</span><span class="sxs-lookup"><span data-stu-id="9cffd-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="9cffd-108">בחר **העבר בעלות על חיוב** עבור המנוי שברצונך להעביר</span><span class="sxs-lookup"><span data-stu-id="9cffd-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="9cffd-109">הזן את כתובת הדואר האלקטרוני של משתמש שהוא מנהל חיוב של החשבון שיהיה הבעלים החדש עבור המנוי ולאחר מכן בחר **שלח בקשת העברה**</span><span class="sxs-lookup"><span data-stu-id="9cffd-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="9cffd-110">המשתמש יקבל דואר אלקטרוני עם הוראות לסקירת בקשת ההעברה.</span><span class="sxs-lookup"><span data-stu-id="9cffd-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="9cffd-111">כדי לאשר את בקשת ההעברה, המשתמש בוחר את הקישור בהודעת הדואר האלקטרוני ועוקב אחר ההוראות.</span><span class="sxs-lookup"><span data-stu-id="9cffd-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="9cffd-112">**הערה** : אם אתה מעביר את בעלות החיוב של המנוי שלך לחשבון של משתמש בדייר אחר של תכלת לספירה, כל הקצאות [בקרת הגישה המבוססות על תפקידים (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)לניהול משאבים במנוי יוסרו לצמיתות.</span><span class="sxs-lookup"><span data-stu-id="9cffd-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="9cffd-113">רק לבעלים החדש תהיה גישה לניהול משאבים במנוי.</span><span class="sxs-lookup"><span data-stu-id="9cffd-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="9cffd-114">לקבלת מידע נוסף, ראה [העברת מנוי למשתמש בדייר אחר של הודעה בנושא תכלת](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9cffd-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9cffd-115">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="9cffd-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="9cffd-116">העברת בעלות על חיוב עבור מנוי של תכלת לחשבון אחר</span><span class="sxs-lookup"><span data-stu-id="9cffd-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="9cffd-117">אודות העברת בעלות על חיוב עבור מנוי תכלת</span><span class="sxs-lookup"><span data-stu-id="9cffd-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="9cffd-118">העברת Visual Studio, Microsoft Network Network (MPN) ושלם במהלך העבודה על Dev/בדיקת מנויים</span><span class="sxs-lookup"><span data-stu-id="9cffd-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="9cffd-119">שאלות נפוצות אודות העברת בעלות</span><span class="sxs-lookup"><span data-stu-id="9cffd-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="9cffd-120">פתרון בעיות בעלות העברה</span><span class="sxs-lookup"><span data-stu-id="9cffd-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
