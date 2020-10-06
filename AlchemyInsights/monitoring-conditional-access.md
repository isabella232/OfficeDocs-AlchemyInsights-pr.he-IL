---
title: ניטור גישה מותנית
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366429"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="20941-102">ניטור הגישה המותנית עבור Exchange</span><span class="sxs-lookup"><span data-stu-id="20941-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="20941-103">משתמשים המיועדים באמצעות גישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="20941-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="20941-104">כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="20941-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="20941-105">אם יש להעריך את המכשיר, הקפד למשתמש לעבור לאפליקציית הפורטל של החברה ולוודא שהיא מופיעה בפורטל החברה.</span><span class="sxs-lookup"><span data-stu-id="20941-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="20941-106">אם היא אינה מופיעה, המשתמש צריך לרשום את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="20941-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="20941-107">בפורטל התכלת, עבור אל כוונון תאימות התקן >.</span><span class="sxs-lookup"><span data-stu-id="20941-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="20941-108">תחת צג, לחץ על תאימות מכשיר.</span><span class="sxs-lookup"><span data-stu-id="20941-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="20941-109">הצג את דוח תאימות המכשירים כדי לוודא שהתקן המשתמש מסומן כתואם.</span><span class="sxs-lookup"><span data-stu-id="20941-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="20941-110">בפורטל התכלת, עבור אל כוונון תאימות התקן >.</span><span class="sxs-lookup"><span data-stu-id="20941-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="20941-111">תחת ניהול, לחץ על מדיניות.</span><span class="sxs-lookup"><span data-stu-id="20941-111">Under Manage, click Policies.</span></span> <span data-ttu-id="20941-112">ברשימת מדיניות התאימות, ודא שהפרופיל מוקצה למכשיר המשתמש שלך.</span><span class="sxs-lookup"><span data-stu-id="20941-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="20941-113">אם לא הוקצה פרופיל, האפשרות ' התאמה ' לא תוכל לאשר את מצב התאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="20941-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="20941-114">ערוך את הקצאת הגישה המותנית של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="20941-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="20941-115">בפורטל ' תכלת ', עבור אל ' **שלחן**  >  **Conditional access**  >  **מדיניות**גישה מותנית '.</span><span class="sxs-lookup"><span data-stu-id="20941-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="20941-116">בחר מדיניות מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="20941-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="20941-117">לחץ על משתמשים וקבוצות.</span><span class="sxs-lookup"><span data-stu-id="20941-117">Click Users and groups.</span></span>
4. <span data-ttu-id="20941-118">כדי לייעד מדיניות מסוימת לאדם כלשהו, הוסף אותם לרשימה כלול.</span><span class="sxs-lookup"><span data-stu-id="20941-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="20941-119">כדי להבטיח שאדם מושמט מהמדיניות, הוסף אותם לרשימת אי-הכללה.</span><span class="sxs-lookup"><span data-stu-id="20941-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="20941-120">קישורים שימושיים:</span><span class="sxs-lookup"><span data-stu-id="20941-120">Helpful links:</span></span>

[<span data-ttu-id="20941-121">מבט כולל על תאימות מכשירים</span><span class="sxs-lookup"><span data-stu-id="20941-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="20941-122">פתרון בעיות ב-CA</span><span class="sxs-lookup"><span data-stu-id="20941-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="20941-123">מדיניות פתרון בעיות</span><span class="sxs-lookup"><span data-stu-id="20941-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="20941-124">ניטור תאימות התקן של כוונון מכשיר</span><span class="sxs-lookup"><span data-stu-id="20941-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="20941-125">הערה: שלבים אלה שימושיים רק בפתרון בעיות בתכונה ' תכלת Active Directory ' גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="20941-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="20941-126">ניתן גם להעביר הסגר על התקן שחוסם את גישת הדואר האלקטרוני שלו באמצעות מדיניות Exchange.</span><span class="sxs-lookup"><span data-stu-id="20941-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="20941-127">ניתן למצוא [כאן](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)מידע נוסף אודות ניהול מכשירים של Exchange.</span><span class="sxs-lookup"><span data-stu-id="20941-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
