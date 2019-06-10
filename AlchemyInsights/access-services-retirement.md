---
title: פרישה שירותים של Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769440"
---
# <a name="access-services-retirement"></a><span data-ttu-id="3992f-102">פרישה שירותים של Access</span><span class="sxs-lookup"><span data-stu-id="3992f-102">Access services retirement</span></span>

<span data-ttu-id="3992f-103">כמו במקור להכריז ב- MC97576, ב- 2017 במרץ, ואנו ממשיכות לקיים תקשורת במהלך השנה האחרונות שירותי Access עובר פרשו מ- Office 365.</span><span class="sxs-lookup"><span data-stu-id="3992f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="3992f-104">השלב הבא בתהליך זה יהיה ההסרה של Access מסדי נתונים של אינטרנט המשתמשים רשימות SharePoint כמקום אחסון הנתונים הבסיסי שלהם.</span><span class="sxs-lookup"><span data-stu-id="3992f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="3992f-105">**כיצד זה משפיע על לי?**</span><span class="sxs-lookup"><span data-stu-id="3992f-105">**How does this affect me?**</span></span>

<span data-ttu-id="3992f-106">החל 2019 ביוני, אנו להפסיק יצירה של מסדי נתונים חדשים של Access ב- SharePoint Online ולכבות את השירות ואת כל apps הנותרים על-ידי 2020 באפריל.</span><span class="sxs-lookup"><span data-stu-id="3992f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="3992f-107">**מה עלי לעשות כדי להתכונן לקראת השינוי?**</span><span class="sxs-lookup"><span data-stu-id="3992f-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="3992f-108">אנו ממליצים ליצור תוכנית המעבר עבור מסדי נתונים של web Access של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="3992f-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="3992f-109">מנהלים באפשרותך להשתמש [סורק יישום SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) לקבלת רשימת מלאי של apps Access משתמש בהם אתרים.</span><span class="sxs-lookup"><span data-stu-id="3992f-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="3992f-110">ישנן מספר דרכים להעברת נתונים במסדי נתונים של Access אינטרנט:</span><span class="sxs-lookup"><span data-stu-id="3992f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="3992f-111">ייבוא למסד נתונים Access מקומי (. ACCDB) או לקובץ Excel.</span><span class="sxs-lookup"><span data-stu-id="3992f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="3992f-112">כמו כן, מומלץ לסייר Microsoft PowerApps כפלטפורמה חלופי כדי ליצור פתרונות עסקיים ללא קוד לאינטרנט ולהתקנים ניידים.</span><span class="sxs-lookup"><span data-stu-id="3992f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>