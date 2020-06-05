---
title: הודעות דוא ל חסרות בהסגר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569230"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="6deba-102">הודעות דוא ל חסרות בהסגר</span><span class="sxs-lookup"><span data-stu-id="6deba-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="6deba-103">מנהלי [מערכת יכולים להציג, לשחרר או למחוק הודעות אלה.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="6deba-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="6deba-104">כדי לפתוח את מרכז התאימות של אבטחה _ אמפר, עבור אל https://protection.office.com .</span><span class="sxs-lookup"><span data-stu-id="6deba-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="6deba-105">כדי לפתוח את דף ההסגר ישירות, עבור אל https://protection.office.com/quarantine .</span><span class="sxs-lookup"><span data-stu-id="6deba-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="6deba-106">באפשרותך לחפש לפי הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="6deba-106">You can search by the following values:</span></span>  

- <span data-ttu-id="6deba-107">**מזהה הודעה**: המזהה הייחודי הגלובלי של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="6deba-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="6deba-108">אם תבחר הודעה ברשימה, ערך **מזהה ההודעה** יופיע בחלונית **הפרטים** הנפתחת שמופיעה.</span><span class="sxs-lookup"><span data-stu-id="6deba-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="6deba-109">למנהלים יש אפשרות להשתמש [במעקב אחר](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) הודעות כדי לחפש את ההודעות ואת ערכי מזהה ההודעה המתאימים להם.</span><span class="sxs-lookup"><span data-stu-id="6deba-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="6deba-110">**כתובת אימייל של השולח**: כתובת אימייל של שולח אחד.</span><span class="sxs-lookup"><span data-stu-id="6deba-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="6deba-111">**כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.</span><span class="sxs-lookup"><span data-stu-id="6deba-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="6deba-112">**נושא**: השתמש בנושא כולו של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="6deba-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="6deba-113">החיפוש אינו תלוי רישיות.</span><span class="sxs-lookup"><span data-stu-id="6deba-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="6deba-114">לאחר שהזנת את קריטריוני החיפוש, לחץ על ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **רענן** לחצן רענון כדי לסנן את התוצאות.  </span><span class="sxs-lookup"><span data-stu-id="6deba-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="6deba-115">יישומוני ה-cmdlet שבהם אתה משתמש כדי להציג ולנהל הודעות וקבצים בהסגר הם:</span><span class="sxs-lookup"><span data-stu-id="6deba-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="6deba-116">הודעת מחיקה-הודעה</span><span class="sxs-lookup"><span data-stu-id="6deba-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="6deba-117">הודעת ייצוא-בהסגר</span><span class="sxs-lookup"><span data-stu-id="6deba-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="6deba-118">הודעת ' קבל-בהסגר '</span><span class="sxs-lookup"><span data-stu-id="6deba-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="6deba-119">הודעת בכיוון [תצוגה מקדימה](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש-cmdlet זה מיועד רק להודעות, לא לקבצים של תוכנות זדוניות מ-ATP עבור SharePoint Online, Onedrive עבור עסקים או צוותים.</span><span class="sxs-lookup"><span data-stu-id="6deba-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="6deba-120">הודעת שחרור בהסגר</span><span class="sxs-lookup"><span data-stu-id="6deba-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)