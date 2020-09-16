---
title: העברה מ-AIP ל-MIP/סימון מאוחד במרכז התאימות
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674327"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="eca58-102">העברה מ-AIP ל-MIP/סימון מאוחד במרכז התאימות</span><span class="sxs-lookup"><span data-stu-id="eca58-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="eca58-103">כדי להעביר מתוויות AIP לתיוג מאוחד במרכז האבטחה והתאימות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="eca58-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="eca58-104">**הפעלת הגנה מפורטל תכלת**</span><span class="sxs-lookup"><span data-stu-id="eca58-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="eca58-105">אם עדיין לא עשית זאת, פתח חלון דפדפן חדש [והיכנס לפורטל תכלת](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="eca58-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="eca58-106">נווט אל להב **הגנת המידע של תכלת** .</span><span class="sxs-lookup"><span data-stu-id="eca58-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="eca58-107">לדוגמה, בתפריט hub, לחץ על **כל השירותים** והתחל להקליד **מידע** בתיבה מסנן.</span><span class="sxs-lookup"><span data-stu-id="eca58-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="eca58-108">בחר **תכלת הגנה על מידע**.</span><span class="sxs-lookup"><span data-stu-id="eca58-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="eca58-109">אם עדיין לא ניגשת ללהב הגנת המידע של ' תכלת ', עיין [בשלבים הנוספים הנוספים](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) להוספת להב זה לפורטל.</span><span class="sxs-lookup"><span data-stu-id="eca58-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="eca58-110">כדי לפתוח את להב הגנת המידע של תכלת, עליך להיות בעל [תוכנית הגנה מפני מידע של תכלת](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) או תוכנית של Office 365 הכוללת ניהול זכויות.</span><span class="sxs-lookup"><span data-stu-id="eca58-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="eca58-111">אם יש לך אחד ממנויים אלה, אך תראה הודעה שאין אפשרות למצוא מנוי חוקי, [פנה לתמיכה של Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) או השתמש בערוצי התמיכה הרגילים שלך.</span><span class="sxs-lookup"><span data-stu-id="eca58-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="eca58-112">אתר את אפשרויות התפריט ' **ניהול** ' ובחר **הפעלת הגנה**.</span><span class="sxs-lookup"><span data-stu-id="eca58-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="eca58-113">לחץ על **הפעל**ולאחר מכן אשר את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="eca58-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="eca58-114">לאחר השלמת ההפעלה, סרגל המידע מציג את **ההפעלה הסתיימה בהצלחה**.</span><span class="sxs-lookup"><span data-stu-id="eca58-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="eca58-115">**העברת תוויות של הגנה על מידע תכלת למרכז התאימות של Office 365 Security &**</span><span class="sxs-lookup"><span data-stu-id="eca58-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="eca58-116">ודא שאתה מחובר כמשתמש עם הרשאת מנהל מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="eca58-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="eca58-117">נווט אל להב **הגנת המידע של תכלת** .</span><span class="sxs-lookup"><span data-stu-id="eca58-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="eca58-118">מתוך אפשרות התפריט ' **ניהול** ', בחר ' **סימון מאוחד**'.</span><span class="sxs-lookup"><span data-stu-id="eca58-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="eca58-119">בהגנה על **מידע תכלת-להב התיוג המאוחד** , לחץ על **הפעל** ובצע את ההוראות המקוונות.</span><span class="sxs-lookup"><span data-stu-id="eca58-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="eca58-120">**הערה**: ודא שיש לך את ההרשאות המתאימות לפני הפעלת ההעברה של מרכז התאימות של אבטחה &.</span><span class="sxs-lookup"><span data-stu-id="eca58-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="eca58-121">ראה מאמרים אלה לקבלת מידע נוסף:</span><span class="sxs-lookup"><span data-stu-id="eca58-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="eca58-122">האם עליך להיות מנהל מערכת כללי כדי לקבוע את התצורה של הגנה מפני מידע של תכלת, או להקצות למנהלי מערכת אחרים?</span><span class="sxs-lookup"><span data-stu-id="eca58-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="eca58-123">מידע חשוב אודות תפקידי ניהול לאחר המעבר למרכז התאימות של אבטחה &.</span><span class="sxs-lookup"><span data-stu-id="eca58-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="eca58-124">לקבלת מידע נוסף אודות AIP כדי לבצע העברת תוויות מאוחדת למרכז האבטחה והתאימות, ראה [העברת תוויות](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="eca58-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
