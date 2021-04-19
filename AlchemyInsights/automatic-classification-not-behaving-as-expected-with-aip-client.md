---
title: סיווג אוטומטי אינו מתנהג כצפוי עם לקוח AIP
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820899"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="c7140-102">סיווג אוטומטי אינו מתנהג כצפוי עם לקוח AIP</span><span class="sxs-lookup"><span data-stu-id="c7140-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="c7140-103">סיווג אוטומטי אינו מתנהג כצפוי, השתמש בקווים המנחים המומלצים הבאים:</span><span class="sxs-lookup"><span data-stu-id="c7140-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="c7140-104">אם אתה נתקל בבעיות בתיוג אוטומטי, ראה כיצד לקבוע את התצורה של תנאים עבור סיווג אוטומטי ומומלץ עבור [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ומה סוגי המידע [הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="c7140-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="c7140-105">בדוק אם אתה משתמש במדיניות טווח שלא נקבעה כראוי: כיצד לקבוע את התצורה של מדיניות Azure Information Protection עבור משתמשים ספציפיים באמצעות [פריטי מדיניות בטווח.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="c7140-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="c7140-106">אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך עם תוויות, ודא שהוא אינו מוגדר `DRMEncryptProperty` כמתואר כאן: הגדרות [הרישום של IRM עבור אבטחה.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="c7140-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="c7140-107">אם השתמשת [בסוגי המידע המוכללים עבור מדיניות](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) Azure Information Protection, ודא שהתוכן שלך תואם לתבנית הצפויה.</span><span class="sxs-lookup"><span data-stu-id="c7140-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="c7140-108">ודא שהתווית מוגדרת כראוי עבור **אוטומטי או** **מומלץ.**</span><span class="sxs-lookup"><span data-stu-id="c7140-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="c7140-109">(**תיוג** אוטומטי זמין עבור כל יישומי Microsoft  365, בעוד שמומלץ זמין עבור כל יישומי Microsoft 365 למעט עבור Outlook.)</span><span class="sxs-lookup"><span data-stu-id="c7140-109">(**Automatic** labeling is available for all Microsoft 365 apps, whereas **Recommended** is available for all Microsoft 365 apps except for Outlook.)</span></span>
6. <span data-ttu-id="c7140-110">לא ניתן להשתמש במיון אוטומטי עבור מסמכים והודעות דואר אלקטרוני עם תווית ידנית או בעבר עם סיווג גבוה יותר.</span><span class="sxs-lookup"><span data-stu-id="c7140-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="c7140-111">לקבלת מידע נוסף, ראה: [אופן ההחלה של תוויות אוטומטיות או מומלצות](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span><span class="sxs-lookup"><span data-stu-id="c7140-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="c7140-112">אם אתה עדיין נתקל בבעיות, אסוף יומני לקוח של Azure Information Protection וצרף את יומני הרישום המיוצאים לכרטיס התמיכה שלך.</span><span class="sxs-lookup"><span data-stu-id="c7140-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="c7140-113">כדי לייצא יומנים של Azure Information Protection:</span><span class="sxs-lookup"><span data-stu-id="c7140-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="c7140-114">פתח מסמך Office או צור הודעת דואר אלקטרוני חדשה ב- Outlook.</span><span class="sxs-lookup"><span data-stu-id="c7140-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="c7140-115">לחץ **על הגנה/רגישות**  >  **עזרה ומשוב.**</span><span class="sxs-lookup"><span data-stu-id="c7140-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="c7140-116">לחץ **על ייצוא יומני רישום**.</span><span class="sxs-lookup"><span data-stu-id="c7140-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="c7140-117">שמור את יומני הרישום במיקום שלך וצרף אותם לבקשת השירות שלך.</span><span class="sxs-lookup"><span data-stu-id="c7140-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="c7140-118">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="c7140-118">For additional information, see:</span></span>

- [<span data-ttu-id="c7140-119">כיצד להגדיר תנאים עבור סיווג אוטומטי ומומלץ עבור Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-119">How to configure conditions for automatic and recommended classification for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [<span data-ttu-id="c7140-120">מדריכי 'כיצד לעשות' עבור תרחישים נפוצים משתמשים ב- Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-120">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [<span data-ttu-id="c7140-121">סקירת התיעוד של Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c7140-122">סקירת מנויים ותכונות של Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="c7140-123">דרישות עבור Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-123">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="c7140-124">ערכת לימוד להתחלה מהירה עבור Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="c7140-125">הורד את לקוח Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c7140-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
