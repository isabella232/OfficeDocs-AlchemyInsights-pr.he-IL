---
title: 'AIP: פריטי מדיניות אינם מתנהגים כמצופה'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663190"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="61f92-102">AIP: פריטי מדיניות אינם מתנהגים כמצופה</span><span class="sxs-lookup"><span data-stu-id="61f92-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="61f92-103">הגנה על מידע תכלת: פריטי מדיניות אינם מתנהגים כמצופה, עיין בסעיפים הבאים לקבלת הנחיות מומלצות עבור בעיות מדיניות שונות:</span><span class="sxs-lookup"><span data-stu-id="61f92-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="61f92-104">אם אתה נתקל בבעיות עם סימונים חזותיים, עיין בנושא [החלת סימונים חזותיים](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="61f92-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="61f92-105">אם אתה נתקל בבעיות בהוספת תוויות אוטומטיות, עיין בנושא [קביעת התצורה של תנאים לסיווג אוטומטי ומומלץ להגנת מידע של תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [ומידע אודות סוגי המידע הרגישים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="61f92-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="61f92-106">אם אתה נתקל בבעיות עם הגנה מקורית/Pfile, עיין [בתצורה של תצורת הקובץ API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="61f92-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="61f92-107">בדוק אם אתה משתמש בפריטי מדיניות הנמצאים בטווח שאינו [מוגדר כהלכה: כיצד לקבוע את התצורה של מדיניות הגנת המידע של תכלת עבור משתמשים ספציפיים באמצעות מדיניות בטווח](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="61f92-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="61f92-108">אם התווית האוטומטית אינה פועלת עבור Outlook בעת צירוף מסמך עם תוויות, ודא ש-DRMEncryptProperty אינו מוגדר כמתואר כאן: [הגדרות רישום של IRM עבור אבטחה](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="61f92-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="61f92-109">אם אתה עדיין נתקל בבעיות, אסוף את יומני הלקוחות של הגנה על מידע תכלת וצרף את יומני הרישום המיוצא לכרטיס זה.</span><span class="sxs-lookup"><span data-stu-id="61f92-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="61f92-110">פתח מסמך Office או צור הודעת דואר אלקטרוני חדשה ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="61f92-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="61f92-111">לחץ על **הגנה/**  >  **עזרה ומשוב**על רגישות.</span><span class="sxs-lookup"><span data-stu-id="61f92-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="61f92-112">לחץ על **יצא יומני רישום**.</span><span class="sxs-lookup"><span data-stu-id="61f92-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="61f92-113">שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת שירות זו.</span><span class="sxs-lookup"><span data-stu-id="61f92-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="61f92-114">משאבים נוספים:</span><span class="sxs-lookup"><span data-stu-id="61f92-114">Additional resources:</span></span>

- [<span data-ttu-id="61f92-115">כיצד להגדיר תווית עבור סימונים חזותיים עבור הגנה על מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="61f92-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="61f92-116">סקירת התיעוד של הגנה על מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="61f92-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="61f92-117">שימוש בתוויות רגישות ביישומי Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="61f92-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

