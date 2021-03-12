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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708675"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="9d467-102">ניטור הגישה המותנית עבור Exchange</span><span class="sxs-lookup"><span data-stu-id="9d467-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="9d467-103">משתמשים המיועדים באמצעות גישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="9d467-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9d467-104">כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="9d467-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="9d467-105">אם יש להעריך את המכשיר, הקפד למשתמש לעבור לאפליקציית הפורטל של החברה ולוודא שהיא מופיעה בפורטל החברה.</span><span class="sxs-lookup"><span data-stu-id="9d467-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9d467-106">אם היא אינה מופיעה, המשתמש צריך לרשום את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="9d467-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="9d467-107">בפורטל ' תכלת ', עבור אל ' כוונון תאימות מכשיר > '.</span><span class="sxs-lookup"><span data-stu-id="9d467-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="9d467-108">תחת צג, לחץ על תאימות מכשיר.</span><span class="sxs-lookup"><span data-stu-id="9d467-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="9d467-109">הצג את דוח תאימות המכשירים כדי לוודא שהתקן המשתמש מסומן כתואם.</span><span class="sxs-lookup"><span data-stu-id="9d467-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="9d467-110">בפורטל ' תכלת ', עבור אל ' כוונון תאימות מכשיר > '.</span><span class="sxs-lookup"><span data-stu-id="9d467-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="9d467-111">תחת ניהול, לחץ על מדיניות.</span><span class="sxs-lookup"><span data-stu-id="9d467-111">Under Manage, click Policies.</span></span> <span data-ttu-id="9d467-112">ברשימת מדיניות התאימות, ודא שהפרופיל מוקצה למכשיר המשתמש שלך.</span><span class="sxs-lookup"><span data-stu-id="9d467-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9d467-113">אם לא הוקצה פרופיל, האפשרות ' התאמה ' לא תוכל לאשר את מצב התאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="9d467-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="9d467-114">ערוך את הקצאת הגישה המותנית של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="9d467-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="9d467-115">בפורטל ' תכלת ', עבור אל ' **שלחן**  >    >  **מדיניות** גישה מותנית '.</span><span class="sxs-lookup"><span data-stu-id="9d467-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="9d467-116">בחר מדיניות מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="9d467-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="9d467-117">לחץ על משתמשים וקבוצות.</span><span class="sxs-lookup"><span data-stu-id="9d467-117">Click Users and groups.</span></span>
4. <span data-ttu-id="9d467-118">כדי לייעד מדיניות מסוימת לאדם כלשהו, הוסף אותם לרשימה כלול.</span><span class="sxs-lookup"><span data-stu-id="9d467-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="9d467-119">כדי להבטיח שאדם מושמט מהמדיניות, הוסף אותם לרשימת אי-הכללה.</span><span class="sxs-lookup"><span data-stu-id="9d467-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="9d467-120">קישורים שימושיים:</span><span class="sxs-lookup"><span data-stu-id="9d467-120">Helpful links:</span></span>

[<span data-ttu-id="9d467-121">מבט כולל על תאימות מכשירים</span><span class="sxs-lookup"><span data-stu-id="9d467-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9d467-122">פתרון בעיות ב-CA</span><span class="sxs-lookup"><span data-stu-id="9d467-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9d467-123">מדיניות פתרון בעיות</span><span class="sxs-lookup"><span data-stu-id="9d467-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="9d467-124">ניטור תאימות התקן של כוונון מכשיר</span><span class="sxs-lookup"><span data-stu-id="9d467-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="9d467-125">הערה: שלבים אלה שימושיים רק בפתרון בעיות בתכונה ' תכלת Active Directory ' גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="9d467-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="9d467-126">ניתן גם להעביר הסגר על התקן שחוסם את גישת הדואר האלקטרוני שלו באמצעות מדיניות Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d467-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="9d467-127">ניתן למצוא מידע נוסף אודות ניהול מכשירים של Exchange [כאן] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="9d467-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
