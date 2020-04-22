---
title: דוחות יומן ביקורת קלאסיים של SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741966"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="c7a86-102">יומני ביקורת של SharePoint ו-OneDrive</span><span class="sxs-lookup"><span data-stu-id="c7a86-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="c7a86-103">יומני ביקורת קלאסיים של SharePoint</span><span class="sxs-lookup"><span data-stu-id="c7a86-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="c7a86-104">ביקורת מדור קודם של SPO הועברה ליומן ביקורת אחיד (רע מ).</span><span class="sxs-lookup"><span data-stu-id="c7a86-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="c7a86-105">כל דוחות הביקורת מהדור הקודם של SPO יהיו מופעל באמצעות רע מ, ואותות הביקורת הישנים הועברו ל-רע מ.</span><span class="sxs-lookup"><span data-stu-id="c7a86-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="c7a86-106">שינויי מפתח:</span><span class="sxs-lookup"><span data-stu-id="c7a86-106">Key changes:</span></span>

* <span data-ttu-id="c7a86-107">זמירה אינו זמין כיכולת.</span><span class="sxs-lookup"><span data-stu-id="c7a86-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="c7a86-108">בחירת אירועים ספציפיים לביקורת אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="c7a86-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="c7a86-109">עיין [במסמך זה](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) לקבלת רשימה מלאה של אירועים מבוקרים הזמינים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="c7a86-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="c7a86-110">אפשרות **המיקום** תחת **דוחות מותאמים אישית** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="c7a86-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="c7a86-111">האפשרות **פתיחה או הורדה של אירועי מסמכים** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="c7a86-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="c7a86-112">קביעת תצורה של הגדרות ביקורת עבור אוסף אתרים</span><span class="sxs-lookup"><span data-stu-id="c7a86-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="c7a86-113">SharePoint ו-OneDrive מודרני יומני ביקורת מאוחד מציות</span><span class="sxs-lookup"><span data-stu-id="c7a86-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="c7a86-114">הפעלה/ביטול של רישום ביקורת אחיד</span><span class="sxs-lookup"><span data-stu-id="c7a86-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="c7a86-115">אין צורך בקביעת תצורה נוספת בתוך SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c7a86-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="c7a86-116">השתמש בחיפוש ביומן ביקורת כדי לבדוק את הפעילות של הקבצים, התיקיות, המשתמשים, ההרשאות:</span><span class="sxs-lookup"><span data-stu-id="c7a86-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="c7a86-117">פעילויות קובץ ועמוד</span><span class="sxs-lookup"><span data-stu-id="c7a86-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="c7a86-118">פעילויות תיקיה</span><span class="sxs-lookup"><span data-stu-id="c7a86-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="c7a86-119">שיתוף וגישה לפעילויות בקשה</span><span class="sxs-lookup"><span data-stu-id="c7a86-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="c7a86-120">פעילויות סנכרון</span><span class="sxs-lookup"><span data-stu-id="c7a86-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="c7a86-121">פעילויות ניהול האתר</span><span class="sxs-lookup"><span data-stu-id="c7a86-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="c7a86-122">לקבלת מידע נוסף אודות אחזור אירועים אלה, ראה [חיפוש ביומן הביקורת](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="c7a86-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
