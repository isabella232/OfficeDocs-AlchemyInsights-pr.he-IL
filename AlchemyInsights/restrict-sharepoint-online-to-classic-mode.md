---
title: להגביל את SharePoint Online במצב קלאסי
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551560"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="5889d-102">להגביל את SharePoint Online במצב קלאסי</span><span class="sxs-lookup"><span data-stu-id="5889d-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="5889d-103">ארגונים מסוימים דורשים עדיין את חוויית במצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="5889d-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="5889d-104">כאשר אין גם כל תוכניות כדי להסיר במצב קלאסי ברמה מדוקדקת, היא אינה אפשרית עוד להגביל את הארגון כולו (דיירים) במצב קלאסי עבור רשימות וספריות.</span><span class="sxs-lookup"><span data-stu-id="5889d-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="5889d-105">המנהל תהיה האפשרויות הבאות כדי לנהל ברשימות ובספריות במצב קלאסי באמצעות בוררים הצטרפות פרטני שאנו מספקים ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="5889d-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="5889d-106">אוסף אתרים</span><span class="sxs-lookup"><span data-stu-id="5889d-106">site collection</span></span>
- <span data-ttu-id="5889d-107">אתר</span><span class="sxs-lookup"><span data-stu-id="5889d-107">site</span></span>
- <span data-ttu-id="5889d-108">רשימה</span><span class="sxs-lookup"><span data-stu-id="5889d-108">list</span></span>
- <span data-ttu-id="5889d-109">ספריה</span><span class="sxs-lookup"><span data-stu-id="5889d-109">library</span></span>

<span data-ttu-id="5889d-110">בנוסף, רשימות המשתמשים בתכונות מסוימות והתאמות אישיות שאינן נתמכות על-ידי מודרנית עדיין להיות שונתה באופן אוטומטי במצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="5889d-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="5889d-111">החל באפריל 1 במאי 2019, התהליך כדי להשבית את רמת דיירים ההצטרפות רשימה מודרני ו ספריות להתחיל ולהמשיך עד 31 במאי 2019.</span><span class="sxs-lookup"><span data-stu-id="5889d-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="5889d-112">הרשימות והספריות הנמצאים במצב קלאסי כתוצאה דיירים opt-out באופן אוטומטי יוסטו כדי מודרניים.</span><span class="sxs-lookup"><span data-stu-id="5889d-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="5889d-113">אם דרוש לך במצב קלאסי נא עיין במידע נוסף [כאן](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) והוראת PnP Powershell [כאן](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) המתאר ואפשרויות של כלים שבהם באפשרותך להשתמש היום לשימוש בחוויית במצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="5889d-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
