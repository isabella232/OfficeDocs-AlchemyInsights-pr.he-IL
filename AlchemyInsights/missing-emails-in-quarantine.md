---
title: הודעות דואר אלקטרוני חסרות בהסגר
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831735"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="16c12-102">הודעות דואר אלקטרוני חסרות בהסגר"</span><span class="sxs-lookup"><span data-stu-id="16c12-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="16c12-103">מנהלי מערכת יכולים [להציג, לשחרר או למחוק הודעות אלה.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="16c12-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="16c12-104">כדי לפתוח את מרכז & האבטחה, עבור אל [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="16c12-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="16c12-105">כדי לפתוח את דף ההסגר ישירות, עבור אל [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="16c12-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="16c12-106">באפשרותך לחפש לפי הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="16c12-106">You can search by the following values:</span></span>  

- <span data-ttu-id="16c12-107">**מזהה הודעה:** המזהה הייחודי הכללי של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="16c12-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="16c12-108">אם תבחר הודעה ברשימה, הערך  **'מזהה הודעה'**  יופיע בחלונית  **הפרטים נשלף**  שמופיעה.</span><span class="sxs-lookup"><span data-stu-id="16c12-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="16c12-109">מנהלי מערכת יכולים להשתמש [במעקב אחר](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) הודעות כדי למצוא הודעות ואת ערכי מזהה ההודעה המתאימים שלהם.</span><span class="sxs-lookup"><span data-stu-id="16c12-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="16c12-110">**כתובת דואר אלקטרוני של** שולח : כתובת דואר אלקטרוני של שולח יחיד.</span><span class="sxs-lookup"><span data-stu-id="16c12-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="16c12-111">**כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.</span><span class="sxs-lookup"><span data-stu-id="16c12-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="16c12-112">**נושא**: השתמש בנושא כולו של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="16c12-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="16c12-113">החיפוש אינו תלוי רישיות.</span><span class="sxs-lookup"><span data-stu-id="16c12-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="16c12-114">לאחר הזנת קריטריוני החיפוש, לחץ על רענן לחצן ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **רענן כדי לסנן** את התוצאות.  </span><span class="sxs-lookup"><span data-stu-id="16c12-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="16c12-115">כלי ה- cmdlet השתמשו כדי להציג ולנהל הודעות וקבצים בהסגר הם:</span><span class="sxs-lookup"><span data-stu-id="16c12-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="16c12-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="16c12-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="16c12-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="16c12-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="16c12-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="16c12-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="16c12-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש- cmdlet זה הוא רק עבור הודעות, ולא קבצי תוכנה זדונית מ- ATP עבור SharePoint Online, OneDrive for Business או Teams.</span><span class="sxs-lookup"><span data-stu-id="16c12-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="16c12-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="16c12-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)