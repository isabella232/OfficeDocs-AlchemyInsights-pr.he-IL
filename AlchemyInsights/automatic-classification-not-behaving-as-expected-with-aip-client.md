---
title: הסיווג האוטומטי אינו מתנהג כמצופה באמצעות לקוח AIP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508377"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="d8991-102">הסיווג האוטומטי אינו מתנהג כמצופה באמצעות לקוח AIP</span><span class="sxs-lookup"><span data-stu-id="d8991-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="d8991-103">הסיווג האוטומטי אינו מתנהג כמצופה, השתמש בהנחיות המומלצות הבאות:</span><span class="sxs-lookup"><span data-stu-id="d8991-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="d8991-104">אם נתקלת בבעיות בתיוג אוטומטי, ראה [כיצד להגדיר תנאים לסיווג אוטומטי ומומלץ עבור הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [ואילו סוגי המידע הרגישים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)מחפשים.</span><span class="sxs-lookup"><span data-stu-id="d8991-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="d8991-105">בדוק אם אתה משתמש במדיניות מתוחם שאינה [מוגדרת כראוי: כיצד לקבוע את תצורת המדיניות ' הגנה מפני מידע ' עבור משתמשים ספציפיים באמצעות מדיניות מתוחם](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="d8991-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="d8991-106">אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך המסומן בתווית, ודא `DRMEncryptProperty` שאינו מוגדר כמתואר כאן: [הגדרות הרישום של IRM עבור אבטחה](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="d8991-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="d8991-107">אם השתמשת [בסוגי המידע המוכללים](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) עבור מדיניות ' הגנת מידע תכלת ', ודא שהתוכן תואם לתבנית הצפויה.</span><span class="sxs-lookup"><span data-stu-id="d8991-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="d8991-108">ודא שהתווית מוגדרת כראוי עבור **אוטומטי** או **מומלץ**.</span><span class="sxs-lookup"><span data-stu-id="d8991-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="d8991-109">(תיוג**אוטומטי** זמין עבור כל יישומי office, בעוד **המומלץ** זמין עבור כל יישומי office למעט Outlook.)</span><span class="sxs-lookup"><span data-stu-id="d8991-109">(**Automatic** labeling is available for all Office apps, whereas **Recommended** is available for all Office apps except for Outlook.)</span></span>
6. <span data-ttu-id="d8991-110">אין באפשרותך להשתמש בסיווג אוטומטי עבור מסמכים ואימיילים שסומנו בעבר באופן ידני או בעבר באופן אוטומטי המסומן בסיווג גבוה יותר.</span><span class="sxs-lookup"><span data-stu-id="d8991-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="d8991-111">לקבלת מידע נוסף, ראה: [החלת תוויות אוטומטיות או מומלצות](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span><span class="sxs-lookup"><span data-stu-id="d8991-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="d8991-112">אם אתם עדיין חווים בעיות, אנא אספו את יומני הלקוחות של הגנת המידע התכלת וחברו את היומנים המיוצאים לכרטיס התמיכה שלכם.</span><span class="sxs-lookup"><span data-stu-id="d8991-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="d8991-113">לייצוא יומני הגנת מידע תכלת:</span><span class="sxs-lookup"><span data-stu-id="d8991-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="d8991-114">פתח מסמך של Office או צור מייל חדש ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="d8991-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="d8991-115">לחץ **Protect/Sensitivity**על  >  **עזרה ומשוב של הגנה**/רגישות.</span><span class="sxs-lookup"><span data-stu-id="d8991-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="d8991-116">לחץ על **ייצוא יומני רישום**.</span><span class="sxs-lookup"><span data-stu-id="d8991-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="d8991-117">שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת השירות שלך.</span><span class="sxs-lookup"><span data-stu-id="d8991-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="d8991-118">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="d8991-118">For additional information, see:</span></span>

- [<span data-ttu-id="d8991-119">כיצד להגדיר תנאים לסיווג אוטומטי ומומלץ להגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-119">How to configure conditions for automatic and recommended classification for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [<span data-ttu-id="d8991-120">מדריכי ' כיצד לעשות ' עבור תרחישים נפוצים המשתמשים בהגנה על מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-120">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [<span data-ttu-id="d8991-121">סקירת התיעוד של הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d8991-122">סקירת מנויים ותכונות של הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="d8991-123">דרישות להגנה מפני מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-123">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="d8991-124">הדרכה מהירה עבור הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="d8991-125">הורד את לקוח הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d8991-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
