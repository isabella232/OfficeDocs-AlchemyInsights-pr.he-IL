---
title: 'AIP: פריטי מדיניות אינם מתנהגים כצפוי'
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821628"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="63574-102">AIP: פריטי מדיניות אינם מתנהגים כצפוי</span><span class="sxs-lookup"><span data-stu-id="63574-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="63574-103">Azure Information Protection: פריטי מדיניות אינם מתנהגים כצפוי, עיין בנושאים הבאים לקבלת קווים מנחים מומלצים עבור בעיות מדיניות שונות:</span><span class="sxs-lookup"><span data-stu-id="63574-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="63574-104">אם אתה נתקל בבעיות עם סימונים חזותיים, עיין [בעת החלת סימונים חזותיים](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="63574-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="63574-105">אם אתה נתקל בבעיות בתיוג אוטומטי, עיין באופן קביעת התצורה של תנאים עבור סיווג אוטומטי ומומלץ עבור [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ומה סוגי המידע [הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="63574-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="63574-106">אם אתה נתקל בבעיות בהגנה מקורית/Pfile, עיין בתצורת [ה- API של הקובץ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="63574-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="63574-107">בדוק אם אתה משתמש במדיניות טווח שלא נקבעה כראוי: כיצד לקבוע את התצורה של מדיניות Azure Information Protection עבור משתמשים ספציפיים באמצעות [פריטי מדיניות בטווח.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="63574-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="63574-108">אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך עם תוויות, ודא ש- DRMEncryptProperty אינו מוגדר כמתואר כאן: הגדרות [הרישום של IRM עבור אבטחה.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="63574-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="63574-109">אם אתה עדיין נתקל בבעיות, אסוף יומני לקוח של Azure Information Protection וצרף את יומני הרישום המיוצאים לכרטיס זה.</span><span class="sxs-lookup"><span data-stu-id="63574-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="63574-110">פתח מסמך Office או צור הודעת דואר אלקטרוני חדשה ב- Outlook.</span><span class="sxs-lookup"><span data-stu-id="63574-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="63574-111">לחץ **על הגנה/רגישות**  >  **עזרה ומשוב.**</span><span class="sxs-lookup"><span data-stu-id="63574-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="63574-112">לחץ **על ייצוא יומני רישום**.</span><span class="sxs-lookup"><span data-stu-id="63574-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="63574-113">שמור את יומני הרישום במיקום שלך וצרף אותם לבקשת שירות זו.</span><span class="sxs-lookup"><span data-stu-id="63574-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="63574-114">משאבים נוספים:</span><span class="sxs-lookup"><span data-stu-id="63574-114">Additional resources:</span></span>

- [<span data-ttu-id="63574-115">כיצד להגדיר תווית עבור סימונים חזותיים עבור Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="63574-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="63574-116">סקירת התיעוד של Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="63574-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="63574-117">שימוש בתוויות רגישות באפליקציות Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="63574-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

