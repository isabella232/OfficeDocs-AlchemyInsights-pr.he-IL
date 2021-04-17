---
title: העברה מ- AIP ל- MIP/Unified Labeling במרכז התאימות
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825372"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="544f4-102">העברה מ- AIP ל- MIP/Unified Labeling במרכז התאימות</span><span class="sxs-lookup"><span data-stu-id="544f4-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="544f4-103">כדי לעבור מתוויות AIP לתיוג מאוחד במרכז האבטחה והתאימות, עשה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="544f4-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="544f4-104">**הפעלת הגנה בפורטל Azure**</span><span class="sxs-lookup"><span data-stu-id="544f4-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="544f4-105">אם עדיין לא עשית זאת, פתח חלון דפדפן חדש [והירשם לפורטל Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="544f4-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="544f4-106">נווט אל **להב Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="544f4-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="544f4-107">לדוגמה, בתפריט Hub, לחץ על **כל השירותים** והתחל **להקליד מידע** בתיבה מסנן.</span><span class="sxs-lookup"><span data-stu-id="544f4-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="544f4-108">בחר **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="544f4-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="544f4-109">אם לא ניגשת ללהב Azure Information Protection בעבר, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) עיין בשלבים הנוספות ה חד-זמניים כדי להוסיף להב זה לפורטל.</span><span class="sxs-lookup"><span data-stu-id="544f4-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="544f4-110">כדי לפתוח את להב Azure Information Protection, עליך לתכן תוכנית [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) או תוכנית Office 365 הכוללת ניהול זכויות.</span><span class="sxs-lookup"><span data-stu-id="544f4-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="544f4-111">אם יש לך אחד מהמינויים הללו, אך אתה רואה הודעה שלא ניתן למצוא מנוי חוקי, פנה [לתמיכה של Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) או השתמש בערוצים הרגילים שלך לתמיכה.</span><span class="sxs-lookup"><span data-stu-id="544f4-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="544f4-112">אתר את **אפשרויות** התפריט ניהול ובחר הפעלת **הגנה**.</span><span class="sxs-lookup"><span data-stu-id="544f4-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="544f4-113">לחץ **על הפעל** ולאחר מכן אשר את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="544f4-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="544f4-114">לאחר השלמת ההפעלה, סרגל המידע מציג את **ההפעלה הסתיימה בהצלחה.**</span><span class="sxs-lookup"><span data-stu-id="544f4-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="544f4-115">**העברת תוויות Azure Information Protection אל Office 365 Security & מרכז התאימות**</span><span class="sxs-lookup"><span data-stu-id="544f4-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="544f4-116">ודא שאתה מחובר כמשתמש בעל הרשאת מנהל מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="544f4-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="544f4-117">נווט אל **להב Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="544f4-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="544f4-118">מתוך אפשרות **התפריט ניהול,** בחר **אחידה תוויות**.</span><span class="sxs-lookup"><span data-stu-id="544f4-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="544f4-119">ב- **Azure Information Protection - Unified label blade,** לחץ על הפעל **ובצע** את ההוראות המקוונות.</span><span class="sxs-lookup"><span data-stu-id="544f4-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="544f4-120">**הערה:** ודא שיש לך את ההרשאות המתאימות לפני הפעלת העברת מרכז & האבטחה.</span><span class="sxs-lookup"><span data-stu-id="544f4-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="544f4-121">עיין במאמרים אלה לקבלת מידע נוסף:</span><span class="sxs-lookup"><span data-stu-id="544f4-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="544f4-122">האם עליך להיות מנהל מערכת כללי כדי לקבוע את התצורה של Azure Information Protection, או האם ניתן להקצות למנהלי מערכת אחרים?</span><span class="sxs-lookup"><span data-stu-id="544f4-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="544f4-123">מידע חשוב אודות תפקידי ניהול לאחר המעבר אל מרכז האבטחה & תאימות.</span><span class="sxs-lookup"><span data-stu-id="544f4-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="544f4-124">לקבלת מידע נוסף על העברת AIP להעברה אחידה של תוויות למרכז האבטחה והתאימות, ראה [העברת תוויות](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="544f4-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
