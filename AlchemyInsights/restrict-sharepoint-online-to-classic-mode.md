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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369774"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="c82d0-102">להגביל את SharePoint Online במצב קלאסי</span><span class="sxs-lookup"><span data-stu-id="c82d0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="c82d0-103">ארגונים מסוימים דורשים עדיין את חוויית במצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="c82d0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="c82d0-104">כאשר אין גם כל תוכניות כדי להסיר במצב קלאסי ברמה מדוקדקת, היא אינה אפשרית עוד להגביל את הארגון כולו (דיירים) במצב קלאסי עבור רשימות וספריות.</span><span class="sxs-lookup"><span data-stu-id="c82d0-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="c82d0-105">המנהל תהיה האפשרויות הבאות כדי לנהל ברשימות ובספריות במצב קלאסי באמצעות בוררים הצטרפות פרטני שאנו מספקים ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c82d0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="c82d0-106">אוסף אתרים</span><span class="sxs-lookup"><span data-stu-id="c82d0-106">site collection</span></span>
- <span data-ttu-id="c82d0-107">אתר</span><span class="sxs-lookup"><span data-stu-id="c82d0-107">site</span></span>
- <span data-ttu-id="c82d0-108">רשימה</span><span class="sxs-lookup"><span data-stu-id="c82d0-108">list</span></span>
- <span data-ttu-id="c82d0-109">ספריה</span><span class="sxs-lookup"><span data-stu-id="c82d0-109">library</span></span>

<span data-ttu-id="c82d0-110">בנוסף, רשימות המשתמשים בתכונות מסוימות והתאמות אישיות שאינן נתמכות על-ידי מודרנית עדיין להיות שונתה באופן אוטומטי במצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="c82d0-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="c82d0-111">החל באפריל 1 במאי 2019, התהליך כדי להשבית את רמת דיירים ההצטרפות רשימה מודרני ו ספריות להתחיל ולהמשיך עד 31 במאי 2019.</span><span class="sxs-lookup"><span data-stu-id="c82d0-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="c82d0-112">הרשימות והספריות הנמצאים במצב קלאסי כתוצאה דיירים opt-out באופן אוטומטי יוסטו כדי מודרניים.</span><span class="sxs-lookup"><span data-stu-id="c82d0-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="c82d0-113">אם דרוש לך במצב קלאסי נא עיין במידע נוסף [כאן](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) והוראת PnP Powershell [כאן](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) המתאר ואפשרויות של כלים שבהם באפשרותך להשתמש היום לשימוש בחוויית במצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="c82d0-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
