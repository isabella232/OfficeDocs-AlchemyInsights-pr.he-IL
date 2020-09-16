---
title: הגבל את SharePoint Online למצב קלאסי
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751423"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="907a2-102">הגבל את SharePoint Online למצב קלאסי</span><span class="sxs-lookup"><span data-stu-id="907a2-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="907a2-103">ארגונים מסוימים עדיין דורשים את חוויית המצב הקלאסי.</span><span class="sxs-lookup"><span data-stu-id="907a2-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="907a2-104">בעוד שאין תוכניות להסרת מצב קלאסי ברמה גרעינית, לא ניתן עוד להגביל ארגון שלם (דייר) למצב קלאסי עבור רשימות וספריות.</span><span class="sxs-lookup"><span data-stu-id="907a2-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="907a2-105">מנהל המערכת יקבל את האפשרויות הבאות כדי לנהל רשימות וספריות בודדות במצב קלאסי באמצעות מתגי הצטרפות משתמשים שאנו מספקים ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="907a2-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="907a2-106">אוסף אתרים</span><span class="sxs-lookup"><span data-stu-id="907a2-106">site collection</span></span>
- <span data-ttu-id="907a2-107">אתר</span><span class="sxs-lookup"><span data-stu-id="907a2-107">site</span></span>
- <span data-ttu-id="907a2-108">רשימה</span><span class="sxs-lookup"><span data-stu-id="907a2-108">list</span></span>
- <span data-ttu-id="907a2-109">ספריה</span><span class="sxs-lookup"><span data-stu-id="907a2-109">library</span></span>

<span data-ttu-id="907a2-110">בנוסף, רשימות המשתמשות בתכונות והתאמות אישיות מסוימות שאינן נתמכות על-ידי המודרני עדיין מועברות באופן אוטומטי למצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="907a2-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="907a2-111">החל מ-1 באפריל 2019, התהליך להפיכת רמת הדייר ללא זמינה מהרשימה המודרנית וספריות יופעלו וימשיכו עד ה-31 במאי 2019.</span><span class="sxs-lookup"><span data-stu-id="907a2-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="907a2-112">הרשימות והספריות הנמצאות במצב קלאסי כתוצאה מבחירת הדיירים מועברות באופן אוטומטי למודרני.</span><span class="sxs-lookup"><span data-stu-id="907a2-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="907a2-113">אם אתה זקוק למצב קלאסי, ראה מידע נוסף [כאן](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) והדרכה של PnP Powershell [כאן](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) המתארות אפשרויות וכלים שבהם באפשרותך להשתמש היום כדי להשתמש בחוויית המצב הקלאסית.</span><span class="sxs-lookup"><span data-stu-id="907a2-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
