---
title: שירותי גישה לגמלאות
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747785"
---
# <a name="access-services-retirement"></a><span data-ttu-id="c3955-102">שירותי גישה לגמלאות</span><span class="sxs-lookup"><span data-stu-id="c3955-102">Access services retirement</span></span>

<span data-ttu-id="c3955-103">כפי שהכרזנו במקור ב-MC97576, במרץ 2017, והמשיך לתקשר בשנה האחרונה שירותי הגישה פרשו מ-Office 365.</span><span class="sxs-lookup"><span data-stu-id="c3955-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="c3955-104">השלב הבא בתהליך זה יהיה ההסרה של מסדי נתונים של Access המשתמשים ברשימות SharePoint כאחסון הנתונים הבסיסי שלהם.</span><span class="sxs-lookup"><span data-stu-id="c3955-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="c3955-105">**? איך זה משפיע עליי**</span><span class="sxs-lookup"><span data-stu-id="c3955-105">**How does this affect me?**</span></span>

<span data-ttu-id="c3955-106">החל יוני 2019, נפסיק את היצירה של מסדי נתונים חדשים של Access ב-SharePoint Online ולסגור את השירות וכל היישומים הנותרים על ידי אפריל 2020.</span><span class="sxs-lookup"><span data-stu-id="c3955-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="c3955-107">**מה עלי לעשות כדי להתכונן לשינוי זה?**</span><span class="sxs-lookup"><span data-stu-id="c3955-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="c3955-108">אנו מעודדים אותך ליצור תוכנית מעבר עבור מסדי הנתונים של הארגון שלך ב-Access.</span><span class="sxs-lookup"><span data-stu-id="c3955-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="c3955-109">למנהלים יש אפשרות להשתמש [בסורק ה-SharePoint Access app](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) כדי לקבל רשימת מלאי של יישומי Access שבהם משתמשים אתרים.</span><span class="sxs-lookup"><span data-stu-id="c3955-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="c3955-110">קיימות מספר דרכים להעברת נתוני מסדי נתונים באינטרנט של Access:</span><span class="sxs-lookup"><span data-stu-id="c3955-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="c3955-111">ייבוא למסד נתונים מקומי של Access (. ACCDB) או לקובץ Excel.</span><span class="sxs-lookup"><span data-stu-id="c3955-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="c3955-112">כמו כן, אנו ממליצים לחקור את Microsoft PowerApps כפלטפורמה חלופית כדי ליצור פתרונות עסקיים ללא קוד עבור מכשירים לאינטרנט ולמכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="c3955-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>