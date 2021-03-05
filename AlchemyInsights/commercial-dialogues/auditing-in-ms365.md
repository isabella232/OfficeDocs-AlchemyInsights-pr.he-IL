---
title: ביקורת ב-Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482368"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="6e6e1-102">ביקורת ב-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6e6e1-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="6e6e1-103">להלן כמה דברים שעליך לדעת אודות ביקורת ב-Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="6e6e1-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="6e6e1-104">פעילויות מנהלי מערכת של Exchange מתבצעות ביקורת כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="6e6e1-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="6e6e1-105">אנו נמצאים בתהליך של הפעלת ביקורת תיבת דואר כברירת מחדל עבור כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="6e6e1-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="6e6e1-106">כדי לקרוא מידע נוסף על כך, לחץ [כאן](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span><span class="sxs-lookup"><span data-stu-id="6e6e1-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="6e6e1-107">עד אז, אם אתה מעוניין בהוראות כדי להפוך אותה לזמינה באופן ידני עבור אדם אחד או ארגון שלם, בחר את לחצן הפעל ביקורת תיבת דואר להלן.</span><span class="sxs-lookup"><span data-stu-id="6e6e1-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="6e6e1-108">תיקיות הדואר של Microsoft 365 ותיבות הדואר הציבוריות אינן תומכות ברישום ביקורת.</span><span class="sxs-lookup"><span data-stu-id="6e6e1-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="6e6e1-109">עבור SharePoint/OneDrive, אין תצורה נוספת הנדרשת לביקורת זמינה.</span><span class="sxs-lookup"><span data-stu-id="6e6e1-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="6e6e1-110">כדי ללמוד באילו פעילויות מתבצעות ביקורת, ראה:</span><span class="sxs-lookup"><span data-stu-id="6e6e1-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="6e6e1-111">פעילויות קובץ</span><span class="sxs-lookup"><span data-stu-id="6e6e1-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="6e6e1-112">פעילויות תיקיה</span><span class="sxs-lookup"><span data-stu-id="6e6e1-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="6e6e1-113">[שיתוף וגישה לפעילויות](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span><span class="sxs-lookup"><span data-stu-id="6e6e1-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="6e6e1-114">לקבלת רשימה של כל הפעילויות המתבצעות ביקורת לפי שירות, ראה פעילויות המתבצעות [ביקורת](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="6e6e1-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
