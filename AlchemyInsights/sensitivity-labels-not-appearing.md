---
title: תוויות רגישות לא מופיעות
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801185"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="28d85-102">תוויות רגישות לא מופיעות</span><span class="sxs-lookup"><span data-stu-id="28d85-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="28d85-103">תוויות רגישות מאפשרות לך לסווג ולסייע בהגנה על התוכן הרגיש.</span><span class="sxs-lookup"><span data-stu-id="28d85-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="28d85-104">ניתן ליצור אותם במרכז התאימות של Microsoft 365, מרכז האבטחה של Microsoft 365 או מרכז התאימות של Microsoft 365 & תחת סיווג > תוויות רגישות.</span><span class="sxs-lookup"><span data-stu-id="28d85-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="28d85-105">לקבלת מידע נוסף אודות תכונה זו, ראה [מבט כולל על תוויות רגישות](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="28d85-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="28d85-106">אם הגדרת את תוויות הרגישות שלך אך לא מופיעות באפליקציות Microsoft 365, בדוק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="28d85-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="28d85-107">ודא שתווית הרגישות [פורסמה](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) למשתמשים ולקבוצות הרצויים.</span><span class="sxs-lookup"><span data-stu-id="28d85-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="28d85-108">ודא שהמשתמש משתמש ביישום התומך בתוויות רגישות-ראה [תוויות רגישות במסמך שלך](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="28d85-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="28d85-109">אם אתה [מעביר את התוויות של הגנה על מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), שים לב לשיקולים המפורטים [כאן](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="28d85-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="28d85-110">תמיכה במניעת אובדן נתונים (DLP): כעת, ניתן להשתמש רק בתוויות שמירה כתנאי במדיניות DLP.</span><span class="sxs-lookup"><span data-stu-id="28d85-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="28d85-111">תמיכה עבור תוויות רגישות במדיניות DLP אינה זמינה עדיין, אך אנו עובדים עליו.</span><span class="sxs-lookup"><span data-stu-id="28d85-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="28d85-112">כאשר הצפנה מופעלת בתווית רגישות, באפשרותך לבחור לבצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="28d85-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="28d85-113">הקצה הרשאות כעת</span><span class="sxs-lookup"><span data-stu-id="28d85-113">Assign permissions now</span></span>
    - <span data-ttu-id="28d85-114">אפשר למשתמשים להקצות הרשאות</span><span class="sxs-lookup"><span data-stu-id="28d85-114">Let users assign permissions</span></span>


<span data-ttu-id="28d85-115">לקבלת מידע נוסף אודות בעיות אפשריות, ראה [בעיות ידועות בתוויות רגישות](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="28d85-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>