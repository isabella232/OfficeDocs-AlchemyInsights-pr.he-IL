---
title: מדיניות הגנת יישומים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423599"
---
# <a name="application-protection-policy"></a><span data-ttu-id="12d4c-102">מדיניות הגנת יישומים</span><span class="sxs-lookup"><span data-stu-id="12d4c-102">Application protection policy</span></span>

<span data-ttu-id="12d4c-103">אם אתה חדש במדיניות הגנת יישומים (APP), עיין [במבט כולל על מדיניות הגנת APP](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="12d4c-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="12d4c-104">כדי להתחיל להשתמש ב-APP, ראה [כיצד ליצור ולהקצות מדיניות הגנה APP](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="12d4c-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="12d4c-105">דרישות מדיניות הגנת יישומים:</span><span class="sxs-lookup"><span data-stu-id="12d4c-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="12d4c-106">למשתמש יש רשיון Intune או EMS.</span><span class="sxs-lookup"><span data-stu-id="12d4c-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="12d4c-107">המשתמש שייך לקבוצה הממוקדת על-ידי מדיניות הגנת יישומים.</span><span class="sxs-lookup"><span data-stu-id="12d4c-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="12d4c-108">רק משתמש אחד בחברה נחתם ליישומים מוגנים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="12d4c-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="12d4c-109">היישום יישם את ה- [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="12d4c-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="12d4c-110">לקבלת רשימה של יישומים התומכים ב-SDK, ראה [יישומים מוגנים של Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="12d4c-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="12d4c-111">פריטי מדיניות חלים לאחר שמשתמש העונה על סימני הדרישות הנ ל לתוך יישום מאופשר Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="12d4c-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="12d4c-112">הדרך הקלה ביותר לקבוע אם מדיניות מוחלת היא על-ידי דרישה שהמשתמש יקבע pin במדיניות.</span><span class="sxs-lookup"><span data-stu-id="12d4c-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="12d4c-113">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="12d4c-113">For more information, see:</span></span>

[<span data-ttu-id="12d4c-114">שאלות נפוצות לגבי האפליקציה/מאמא</span><span class="sxs-lookup"><span data-stu-id="12d4c-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="12d4c-115">כיצד לאמת את הגדרת מדיניות הגנת האפליקציה שלך</span><span class="sxs-lookup"><span data-stu-id="12d4c-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="12d4c-116">הבנת מדיניות הגנת האפליקציה תזמון מסירה</span><span class="sxs-lookup"><span data-stu-id="12d4c-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="12d4c-117">כיצד לנטר מדיניות הגנת יישומים</span><span class="sxs-lookup"><span data-stu-id="12d4c-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)