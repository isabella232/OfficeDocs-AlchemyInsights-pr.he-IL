---
title: פרישת שירותים של Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698683"
---
# <a name="access-services-retirement"></a><span data-ttu-id="a5371-102">פרישת שירותים של Access</span><span class="sxs-lookup"><span data-stu-id="a5371-102">Access services retirement</span></span>

<span data-ttu-id="a5371-103">כפי שהכרזתי במקור ב-MC97576, במרץ 2017, והמשכנו לקיים תקשורת במהלך השנה החולפת של Access שירותי הגישה מפורשים.</span><span class="sxs-lookup"><span data-stu-id="a5371-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="a5371-104">השלב הבא בתהליך זה יהיה הסרת מסדי נתונים של Access המשתמשים ברשימות SharePoint כאחסון הנתונים המשמש כבסיס.</span><span class="sxs-lookup"><span data-stu-id="a5371-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="a5371-105">**כיצד זה משפיע עלי?**</span><span class="sxs-lookup"><span data-stu-id="a5371-105">**How does this affect me?**</span></span>

<span data-ttu-id="a5371-106">החל מיוני 2019, אנו נעצור את היצירה של מסדי נתונים חדשים של Access ב-SharePoint Online ונכבה את השירות ואת כל היישומים הנותרים על-ידי אפריל 2020.</span><span class="sxs-lookup"><span data-stu-id="a5371-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="a5371-107">**מה עליי לעשות כדי להתכונן לשינוי זה?**</span><span class="sxs-lookup"><span data-stu-id="a5371-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="a5371-108">אנו ממליצים לך ליצור תוכנית מעבר עבור מסדי הנתונים באינטרנט של Access בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="a5371-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="a5371-109">מנהלי מערכת יכולים להשתמש [בסורק היישומים של SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) כדי לקבל מלאי של יישומי Access שבהם משתמש האתרים.</span><span class="sxs-lookup"><span data-stu-id="a5371-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="a5371-110">קיימות כמה דרכים להעברת נתונים של מסדי נתונים באינטרנט של Access:</span><span class="sxs-lookup"><span data-stu-id="a5371-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="a5371-111">ייבוא למסד נתונים מקומי של Access (. ACCDB) או לקובץ Excel.</span><span class="sxs-lookup"><span data-stu-id="a5371-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="a5371-112">כמו כן, אנו ממליצים לחקור את Microsoft PowerApps כפלטפורמה חלופית כדי ליצור פתרונות עסקיים ללא קוד עבור מכשירים באינטרנט ובמכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="a5371-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>