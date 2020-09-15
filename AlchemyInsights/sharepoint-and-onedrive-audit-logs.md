---
title: דוחות יומן ביקורת קלאסיים של SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662209"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="ecb6f-102">יומני ביקורת של SharePoint ו-OneDrive</span><span class="sxs-lookup"><span data-stu-id="ecb6f-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="ecb6f-103">יומני ביקורת קלאסיים של SharePoint</span><span class="sxs-lookup"><span data-stu-id="ecb6f-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="ecb6f-104">ביקורת מדור קודם של SPO הועברה ליומן ביקורת מאוחד (רע מ).</span><span class="sxs-lookup"><span data-stu-id="ecb6f-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="ecb6f-105">כל דוחות הביקורת המורשית של SPO מופעלים כעת באמצעות רע מ, והאיתותים של ביקורת מדור קודם הועברו ל-רע מ.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="ecb6f-106">שינויים במפתח:</span><span class="sxs-lookup"><span data-stu-id="ecb6f-106">Key changes:</span></span>

* <span data-ttu-id="ecb6f-107">חיתוך אינו זמין כיכולת.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="ecb6f-108">בחירת אירועים ספציפיים לביקורת אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="ecb6f-109">עיין [במסמך זה](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) לקבלת רשימה מלאה של אירועים הניתנים לביקורת כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="ecb6f-110">האפשרות **מיקום** תחת **דוחות מותאמים אישית** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="ecb6f-111">האפשרות **פתיחה או הורדה של אירועים מסמכים** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="ecb6f-112">קביעת תצורה של הגדרות ביקורת עבור אוסף אתרים</span><span class="sxs-lookup"><span data-stu-id="ecb6f-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="ecb6f-113">יומני ביקורת מאוחדים של SharePoint ו-OneDrive מודרניים מתאימות</span><span class="sxs-lookup"><span data-stu-id="ecb6f-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="ecb6f-114">הפעלה/ביטול של רישום ביקורת מאוחדת</span><span class="sxs-lookup"><span data-stu-id="ecb6f-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="ecb6f-115">אין צורך בקביעת תצורה נוספת בתוך SharePoint או ב-OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ecb6f-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="ecb6f-116">השתמש בחיפוש רישום ביקורת כדי לבדוק את הפעילות של הקבצים, התיקיות, המשתמשים, המשתמשים או ההרשאות:</span><span class="sxs-lookup"><span data-stu-id="ecb6f-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="ecb6f-117">פעילויות קובץ ועמוד</span><span class="sxs-lookup"><span data-stu-id="ecb6f-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="ecb6f-118">פעילויות תיקיה</span><span class="sxs-lookup"><span data-stu-id="ecb6f-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="ecb6f-119">פעילויות בקשת שיתוף וגישה</span><span class="sxs-lookup"><span data-stu-id="ecb6f-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="ecb6f-120">פעילויות סינכרון</span><span class="sxs-lookup"><span data-stu-id="ecb6f-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="ecb6f-121">פעילויות ניהול אתר</span><span class="sxs-lookup"><span data-stu-id="ecb6f-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="ecb6f-122">לקבלת מידע נוסף אודות אופן האחזור של אירועים אלה, ראה [חיפוש ביומן הביקורת](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ecb6f-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
