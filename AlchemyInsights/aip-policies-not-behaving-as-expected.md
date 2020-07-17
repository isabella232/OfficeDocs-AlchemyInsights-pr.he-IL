---
title: 'AIP: מדיניות שאינה מתנהגת כמצופה'
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
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506559"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="d9298-102">AIP: מדיניות שאינה מתנהגת כמצופה</span><span class="sxs-lookup"><span data-stu-id="d9298-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="d9298-103">הגנת מידע תכלת: מדיניות שאינה מתנהגת כמצופה, עיין בהוראות הבאות לקבלת הנחיות מומלצות לסוגיות מדיניות שונות:</span><span class="sxs-lookup"><span data-stu-id="d9298-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="d9298-104">אם נתקלת בבעיות בסימונים חזותיים, עיין [במועד ההחלה של סימונים חזותיים](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="d9298-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="d9298-105">אם אתה נתקל בבעיות עם תיוג אוטומטי, עיין [באופן ההגדרה של תנאים לסיווג אוטומטי ומומלץ עבור הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [ואילו סוגי המידע הרגישים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)מחפשים.</span><span class="sxs-lookup"><span data-stu-id="d9298-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="d9298-106">אם נתקלת בבעיות בהגנה על מקורי/Pfile, עיין [בתצורת ה-API של הקובץ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="d9298-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="d9298-107">בדוק אם אתה משתמש במדיניות מתוחם שאינה [מוגדרת כראוי: כיצד לקבוע את תצורת המדיניות ' הגנה מפני מידע ' עבור משתמשים ספציפיים באמצעות מדיניות מתוחם](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="d9298-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="d9298-108">אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך המסומן בתווית, ודא שהמאפיין DRMEncryptProperty אינו מוגדר כמתואר כאן: [הגדרות הרישום של IRM עבור אבטחה](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="d9298-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="d9298-109">אם עדיין נתקלת בבעיות, נא לאסוף את יומני הלקוחות של הגנת המידע התכלת ולצרף את היומנים המיוצאים לכרטיס זה.</span><span class="sxs-lookup"><span data-stu-id="d9298-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="d9298-110">פתח מסמך של Office או צור מייל חדש ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="d9298-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="d9298-111">לחץ **Protect/Sensitivity**על  >  **עזרה ומשוב של הגנה**/רגישות.</span><span class="sxs-lookup"><span data-stu-id="d9298-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="d9298-112">לחץ על **ייצוא יומני רישום**.</span><span class="sxs-lookup"><span data-stu-id="d9298-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="d9298-113">שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת שירות זו.</span><span class="sxs-lookup"><span data-stu-id="d9298-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="d9298-114">משאבים נוספים:</span><span class="sxs-lookup"><span data-stu-id="d9298-114">Additional resources:</span></span>

- [<span data-ttu-id="d9298-115">כיצד להגדיר תווית עבור סימונים חזותיים עבור הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d9298-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="d9298-116">סקירת התיעוד של הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d9298-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d9298-117">שימוש בתוויות רגישות ביישומי Office</span><span class="sxs-lookup"><span data-stu-id="d9298-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

