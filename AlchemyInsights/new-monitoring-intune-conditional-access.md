---
title: הצג גישה מותנית של ' שלחן '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427928"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="6100b-102">הצג גישה מותנית של ' שלחן '</span><span class="sxs-lookup"><span data-stu-id="6100b-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="6100b-103">משתמשים המיועדים באמצעות גישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="6100b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6100b-104">כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="6100b-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="6100b-105">אם יש להעריך את המכשיר, הקפד למשתמש לעבור לאפליקציית הפורטל של החברה ולוודא שהיא מופיעה בפורטל החברה.</span><span class="sxs-lookup"><span data-stu-id="6100b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6100b-106">אם היא אינה מופיעה, על המשתמש לרשום את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="6100b-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="6100b-107">בפורטל התכלת, עבור אל **כוונון**  >  **תאימות התקן**.</span><span class="sxs-lookup"><span data-stu-id="6100b-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="6100b-108">כדי להציג את דוח תאימות המכשירים כדי לוודא שהתקן המשתמש מסומן כתואם, תחת **צג**, לחץ על **תאימות מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="6100b-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="6100b-109">בפורטל התכלת, עבור אל **כוונון**  >  **תאימות התקן**.</span><span class="sxs-lookup"><span data-stu-id="6100b-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="6100b-110">תחת **ניהול,** לחץ על **מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="6100b-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="6100b-111">ברשימת מדיניות התאימות, ודא שהפרופיל מוקצה למכשיר המשתמש שלך.</span><span class="sxs-lookup"><span data-stu-id="6100b-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6100b-112">אם לא הוקצה פרופיל, האפשרות ' התאמה ' לא תוכל לאשר את מצב התאימות של ההתקן.</span><span class="sxs-lookup"><span data-stu-id="6100b-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="6100b-113">ערוך את הקצאת הגישה המותנית של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="6100b-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="6100b-114">בפורטל תכלת, נווט כדי **לכוונן**  >    >  **מדיניות** גישה מותנית, בחר מדיניות מתוך הרשימה ולחץ על **משתמשים וקבוצות**.</span><span class="sxs-lookup"><span data-stu-id="6100b-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="6100b-115">כדי לייעד מדיניות מסוימת לאדם כלשהו, הוסף אותם **לרשימה כלול**.</span><span class="sxs-lookup"><span data-stu-id="6100b-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="6100b-116">כדי להבטיח שאדם מושמט מהמדיניות, הוסף אותם **לרשימת אי-הכללה**.</span><span class="sxs-lookup"><span data-stu-id="6100b-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="6100b-117">**קישורים שימושיים:**</span><span class="sxs-lookup"><span data-stu-id="6100b-117">**Helpful links:**</span></span>

- [<span data-ttu-id="6100b-118">מבט כולל על תאימות מכשירים</span><span class="sxs-lookup"><span data-stu-id="6100b-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="6100b-119">פתרון בעיות ב-CA</span><span class="sxs-lookup"><span data-stu-id="6100b-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="6100b-120">מדיניות פתרון בעיות</span><span class="sxs-lookup"><span data-stu-id="6100b-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="6100b-121">ניטור תאימות התקן של כוונון מכשיר</span><span class="sxs-lookup"><span data-stu-id="6100b-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="6100b-122">שלבים אלה שימושיים רק בפתרון בעיות בתכונה ' תכלת Active Directory ' גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="6100b-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="6100b-123">ניתן גם להעביר הסגר על התקן שחוסם את גישת הדואר האלקטרוני שלו באמצעות מדיניות Exchange.</span><span class="sxs-lookup"><span data-stu-id="6100b-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="6100b-124">ניתן למצוא [**כאן**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))מידע נוסף אודות ניהול מכשירים של Exchange.</span><span class="sxs-lookup"><span data-stu-id="6100b-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
