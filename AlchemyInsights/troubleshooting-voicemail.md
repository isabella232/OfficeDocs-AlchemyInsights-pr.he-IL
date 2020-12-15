---
title: 'פתרון בעיות בדואר קולי '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677963"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="feeca-102">פתרון בעיות בדואר קולי</span><span class="sxs-lookup"><span data-stu-id="feeca-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="feeca-103">ודא שהתכונה ' תפוס על עסוק ' היא מכוונת.</span><span class="sxs-lookup"><span data-stu-id="feeca-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="feeca-104">אם תכונה זו אינה נחוצה במשתמש זה:</span><span class="sxs-lookup"><span data-stu-id="feeca-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="feeca-105">עבור אל [מרכז הניהול של teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="feeca-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="feeca-106">במסילה הימנית   >  , נווט **במדיניות**  >  השיחות הקוליות **ניהול מדיניות** **במדיניות השיחות**.</span><span class="sxs-lookup"><span data-stu-id="feeca-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="feeca-107">בחר **נהל משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="feeca-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="feeca-108">חפש את המשתמש ושנה את מדיניות השיחות לאדם **שעסוק ב-עסוק זמין כאשר אתה בשיחה** **כבויה**.</span><span class="sxs-lookup"><span data-stu-id="feeca-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="feeca-109">לחץ על **'החל'**.</span><span class="sxs-lookup"><span data-stu-id="feeca-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="feeca-110">שינויים בפריטי מדיניות יכולים להימשך עד 24 שעות כדי לשכפל.</span><span class="sxs-lookup"><span data-stu-id="feeca-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="feeca-111">לקבלת מידע נוסף אודות תכונה זו, עיין במאמר: [עסוק ב-עסוק זמין במהלך שיחה](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="feeca-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
