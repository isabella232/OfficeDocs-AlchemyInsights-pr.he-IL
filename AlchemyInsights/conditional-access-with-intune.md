---
title: גישה מותנית עם Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931432"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="3c05f-102">גישה מותנית עם Intune</span><span class="sxs-lookup"><span data-stu-id="3c05f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="3c05f-103">שימוש **בגישה מותנית** עם Intune דורש 3 שלבים:</span><span class="sxs-lookup"><span data-stu-id="3c05f-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="3c05f-104">צור **מדיניות תאימות** ([דמוי אדם](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) כדי להגדיר הגדרות שחייבות להיות מולאו לפני שההתקן נחשב לתואם.</span><span class="sxs-lookup"><span data-stu-id="3c05f-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="3c05f-105">לדוגמה, על התקן להיות בעל pin של 6 ספרות לפחות לפני שהוא נחשב לתואם.</span><span class="sxs-lookup"><span data-stu-id="3c05f-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="3c05f-106">צור **מדיניות גישה מותנית** המגדירה אילו משאבים מוגנים ואילו תנאים יש להכיר כדי לגשת למשאבים אלה.</span><span class="sxs-lookup"><span data-stu-id="3c05f-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="3c05f-107">[לדוגמה,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) על התקן להיות תואם לפני הגישה לדואר אלקטרוני של חברה.</span><span class="sxs-lookup"><span data-stu-id="3c05f-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="3c05f-108">ודא **שמדיניות התאימות** **ופריטי מדיניות הגישה המותנים** מיועדים לקבוצות המשתמשים הרצויות.</span><span class="sxs-lookup"><span data-stu-id="3c05f-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="3c05f-109">הדבר עשוי לדרוש יצירת קבוצות מסוימות של משתמשים בספריית הפעילות התכלת.</span><span class="sxs-lookup"><span data-stu-id="3c05f-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="3c05f-110">**קישורים מועילים:**</span><span class="sxs-lookup"><span data-stu-id="3c05f-110">**Helpful links:**</span></span>

[<span data-ttu-id="3c05f-111">סקירת תאימות התקנים</span><span class="sxs-lookup"><span data-stu-id="3c05f-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="3c05f-112">פתרון בעיות של CA</span><span class="sxs-lookup"><span data-stu-id="3c05f-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="3c05f-113">מדיניות פתרון בעיות</span><span class="sxs-lookup"><span data-stu-id="3c05f-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="3c05f-114">כדי להגן על דואר אלקטרוני (Exchange online) מפני גישה על-ידי התקנים שאינם תואמים, יש לעקוב אחר שני המסמכים:</span><span class="sxs-lookup"><span data-stu-id="3c05f-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="3c05f-115">הגן על גישה לדואר אלקטרוני ממכשירים באמצעות המלווים</span><span class="sxs-lookup"><span data-stu-id="3c05f-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="3c05f-116">הגן על גישה לדואר אלקטרוני ממכשירים באמצעות לקוחות אימות מודרניים כמו Outlook</span><span class="sxs-lookup"><span data-stu-id="3c05f-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)