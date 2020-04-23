---
title: הגבל את SharePoint Online למצב קלאסי
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742470"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="32ec7-102">הגבל את SharePoint Online למצב קלאסי</span><span class="sxs-lookup"><span data-stu-id="32ec7-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="32ec7-103">ארגונים מסוימים עדיין דורשים את חוויית המצב הקלאסי.</span><span class="sxs-lookup"><span data-stu-id="32ec7-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="32ec7-104">אמנם אין תוכניות להסיר מצב קלאסי ברמה הגרעינית, אין עוד אפשרות להגביל את הארגון כולו (דייר) למצב הקלאסי עבור רשימות וספריות.</span><span class="sxs-lookup"><span data-stu-id="32ec7-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="32ec7-105">למנהל יהיו האפשרויות הבאות לניהול רשימות וספריות בודדות במצב קלאסי באמצעות מתגי הצטרפות מבודדים שאנו מספקים ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="32ec7-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="32ec7-106">אוסף אתרים</span><span class="sxs-lookup"><span data-stu-id="32ec7-106">site collection</span></span>
- <span data-ttu-id="32ec7-107">אתר</span><span class="sxs-lookup"><span data-stu-id="32ec7-107">site</span></span>
- <span data-ttu-id="32ec7-108">רשימה</span><span class="sxs-lookup"><span data-stu-id="32ec7-108">list</span></span>
- <span data-ttu-id="32ec7-109">ספריה</span><span class="sxs-lookup"><span data-stu-id="32ec7-109">library</span></span>

<span data-ttu-id="32ec7-110">בנוסף, רשימות המשתמשות בתכונות והתאמות אישיות מסוימות שאינן נתמכות על-ידי המודרניות עדיין מוחלפות באופן אוטומטי למצב קלאסי.</span><span class="sxs-lookup"><span data-stu-id="32ec7-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="32ec7-111">החל באפריל 1, 2019, התהליך להשבית את רמת הדייר מחוץ לרשימה המודרנית הספריות יתחילו ולהמשיך במאי 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="32ec7-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="32ec7-112">הרשימות והספריות הנמצאות במצב קלאסי כתוצאה מבחירת הדיירים החוצה באופן אוטומטי, משתנה למודרני.</span><span class="sxs-lookup"><span data-stu-id="32ec7-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="32ec7-113">אם דרוש לך מצב קלאסי נא עיין במידע נוסף [כאן](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) והוראת PnP Powershell [כאן](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) המתארת אפשרויות וכלים שבהם באפשרותך להשתמש כיום כדי להשתמש בחוויית המצב הקלאסי.</span><span class="sxs-lookup"><span data-stu-id="32ec7-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
