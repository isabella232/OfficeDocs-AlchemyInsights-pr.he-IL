---
title: ניהול רישום ביומן
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745730"
---
# <a name="manage-journaling"></a><span data-ttu-id="f96c8-102">ניהול רישום ביומן</span><span class="sxs-lookup"><span data-stu-id="f96c8-102">Manage journaling</span></span>

<span data-ttu-id="f96c8-103">רישום ביומן יכול לעזור לארגון שלך להגיב לדרישות תאימות משפטיות, רגולטוריות וארגוניות על-ידי הקלטת תקשורת נכנסת ויוצאת לדואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="f96c8-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="f96c8-104">שים לב:</span><span class="sxs-lookup"><span data-stu-id="f96c8-104">Keep in mind:</span></span>

* <span data-ttu-id="f96c8-105">עליך להיות בעל הרשאות ניהול [ארגוני](https://go.microsoft.com/fwlink/?linkid=2115259) וניהול [רשומות](https://go.microsoft.com/fwlink/?linkid=2115469) כדי שתוכל לנהל את הרישום ביומן.</span><span class="sxs-lookup"><span data-stu-id="f96c8-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="f96c8-106">עליך להיות בעל תיבת דואר של יומן ולחלופין, באפשרותך להגדיר תיבת דואר חלופית של רישום ביומן.</span><span class="sxs-lookup"><span data-stu-id="f96c8-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="f96c8-107">לקבלת מידע נוסף, ראה [קביעת תצורה של רישום ביומן ב-Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="f96c8-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="f96c8-108">ב-Exchange Online, קיימת מגבלה על מספר כללי היומן שניתן ליצור.</span><span class="sxs-lookup"><span data-stu-id="f96c8-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="f96c8-109">לקבלת פרטים, ראה [מגבלות כללי של יומן, תעבורה ותיבת דואר נכנס](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="f96c8-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="f96c8-110">Exchange Online אינו תומך בהעברת דוחות יומן לתיבת דואר של Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f96c8-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="f96c8-111">עליך לציין את כתובת הדואר האלקטרוני של מערכת אחסון מקומית או שירות אחסון בארכיון של ספק חיצוני כתיבת הדואר של הרישום.</span><span class="sxs-lookup"><span data-stu-id="f96c8-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
