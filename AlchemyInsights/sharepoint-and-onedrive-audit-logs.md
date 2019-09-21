---
title: דוחות יומן ביקורת קלאסיים של SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068024"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="e25ff-102">יומני ביקורת של SharePoint ו-OneDrive</span><span class="sxs-lookup"><span data-stu-id="e25ff-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="e25ff-103">**SharePoint ו-OneDrive מודרני יומני ביקורת מאוחד מציות**</span><span class="sxs-lookup"><span data-stu-id="e25ff-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="e25ff-104">הפעלה/ביטול של רישום ביקורת אחיד</span><span class="sxs-lookup"><span data-stu-id="e25ff-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="e25ff-105">אין צורך בקביעת תצורה נוספת בתוך SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e25ff-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="e25ff-106">השתמש בחיפוש ביומן ביקורת כדי לבדוק את הפעילות של הקבצים, התיקיות, המשתמשים, ההרשאות:</span><span class="sxs-lookup"><span data-stu-id="e25ff-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="e25ff-107">פעילויות קובץ ועמוד</span><span class="sxs-lookup"><span data-stu-id="e25ff-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="e25ff-108">פעילויות תיקיה</span><span class="sxs-lookup"><span data-stu-id="e25ff-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="e25ff-109">שיתוף וגישה לפעילויות בקשה</span><span class="sxs-lookup"><span data-stu-id="e25ff-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="e25ff-110">פעילויות סנכרון</span><span class="sxs-lookup"><span data-stu-id="e25ff-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="e25ff-111">פעילויות ניהול האתר</span><span class="sxs-lookup"><span data-stu-id="e25ff-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="e25ff-112">לקבלת מידע נוסף אודות אחזור אירועים אלה, ראה [חיפוש ביומן הביקורת](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="e25ff-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="e25ff-113">**יומני ביקורת קלאסיים של SharePoint**</span><span class="sxs-lookup"><span data-stu-id="e25ff-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="e25ff-114">העברנו ביקורת מדור קודם של SPO ליומן ביקורת אחיד (רע מ).</span><span class="sxs-lookup"><span data-stu-id="e25ff-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="e25ff-115">זה בעצם אומר כי כל דוחות ביקורת מורשת SPO כעת יהיה מופעל באמצעות רע מ, ואת אותות ביקורת מדור קודם הועברו רע מ.</span><span class="sxs-lookup"><span data-stu-id="e25ff-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="e25ff-116">שינויי מפתח:</span><span class="sxs-lookup"><span data-stu-id="e25ff-116">Key changes:</span></span>

- <span data-ttu-id="e25ff-117">זמירה כיכולת אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="e25ff-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="e25ff-118">המקטע שבו תבחר אירועים ספציפיים לביקורת אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="e25ff-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="e25ff-119">נא עיין [במסמך זה](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) לקבלת רשימה מלאה של אירועים מבוקרים הזמינים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="e25ff-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="e25ff-120">האפשרות "מיקום" תחת **דוחות מותאמים אישית** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="e25ff-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="e25ff-121">אירועים "פתיחה או הורדה של מסמכים" אינם זמינים.</span><span class="sxs-lookup"><span data-stu-id="e25ff-121">“Opening or downloading documents” events is NOT available.</span></span> 

