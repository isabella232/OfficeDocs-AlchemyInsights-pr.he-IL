---
title: גישה מותנית עם כוונון
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704787"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="dd02f-102">גישה מותנית עם כוונון</span><span class="sxs-lookup"><span data-stu-id="dd02f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="dd02f-103">שימוש  **בגישה מותנית**  עם האפשרות ' כוונון ' דורש שלושה שלבים:</span><span class="sxs-lookup"><span data-stu-id="dd02f-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="dd02f-104">צור  **מדיניות תאימות**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) כדי להגדיר הגדרות שיש לעמוד בהן לפני שההתקן ייחשב כתואם.</span><span class="sxs-lookup"><span data-stu-id="dd02f-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="dd02f-105">לדוגמה, התקן חייב לכלול pin של 6 ספרות לפחות לפני שהוא נחשב לתואם.</span><span class="sxs-lookup"><span data-stu-id="dd02f-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="dd02f-106">צור **מדיניות גישה מותנית**  המגדירה אילו משאבים מוגנים, ואילו תנאים דרושים לפגישה כדי לגשת למשאבים אלה.</span><span class="sxs-lookup"><span data-stu-id="dd02f-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="dd02f-107">[לדוגמה,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  התקן חייב להיות תואם לפני הגישה לדואר אלקטרוני של החברה.</span><span class="sxs-lookup"><span data-stu-id="dd02f-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="dd02f-108">ודא **שפריטי מדיניות התאימות**  **ומדיניות גישה מותנית**  מיועדים לקבוצות המשתמשים הרצויות.</span><span class="sxs-lookup"><span data-stu-id="dd02f-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="dd02f-109">פעולה זו עשויה לדרוש יצירת קבוצות ספציפיות של משתמשים ב-תכלת Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dd02f-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="dd02f-110">**קישורים שימושיים:**</span><span class="sxs-lookup"><span data-stu-id="dd02f-110">**Helpful links:**</span></span>

[<span data-ttu-id="dd02f-111">מבט כולל על תאימות מכשירים</span><span class="sxs-lookup"><span data-stu-id="dd02f-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="dd02f-112">פתרון בעיות ב-CA</span><span class="sxs-lookup"><span data-stu-id="dd02f-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="dd02f-113">מדיניות פתרון בעיות</span><span class="sxs-lookup"><span data-stu-id="dd02f-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="dd02f-114">כדי להגן על דואר אלקטרוני (Exchange online) מ-access על-ידי מכשירים שאינם תואמים, יש לעקוב אחר שני המסמכים:</span><span class="sxs-lookup"><span data-stu-id="dd02f-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="dd02f-115">הגנה על גישה לדואר אלקטרוני ממכשירים המשתמשים במלווים</span><span class="sxs-lookup"><span data-stu-id="dd02f-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="dd02f-116">הגנה על גישה לדואר אלקטרוני ממכשירים באמצעות לקוחות אימות מודרניים כגון Outlook</span><span class="sxs-lookup"><span data-stu-id="dd02f-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)