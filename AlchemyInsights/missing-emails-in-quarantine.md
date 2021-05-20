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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539825"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="25c0d-102">הודעות דואר אלקטרוני חסרות בהסגר"</span><span class="sxs-lookup"><span data-stu-id="25c0d-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="25c0d-103">מנהלי מערכת יכולים [להציג, לשחרר או למחוק הודעות אלה.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="25c0d-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="25c0d-104">כדי לפתוח את מרכז & האבטחה, עבור אל [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="25c0d-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="25c0d-105">כדי לפתוח את דף ההסגר ישירות, עבור אל [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="25c0d-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="25c0d-106">באפשרותך לחפש לפי הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="25c0d-106">You can search by the following values:</span></span>  

- <span data-ttu-id="25c0d-107">**מזהה הודעה:** המזהה הייחודי הכללי של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="25c0d-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="25c0d-108">אם תבחר הודעה ברשימה, הערך  **'מזהה הודעה'**  יופיע בחלונית  **הפרטים נשלף**  שמופיעה.</span><span class="sxs-lookup"><span data-stu-id="25c0d-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="25c0d-109">מנהלי מערכת יכולים להשתמש [במעקב אחר](/microsoft-365/security/office-365-security/message-trace-scc) הודעות כדי למצוא הודעות ואת ערכי מזהה ההודעה המתאימים שלהם.</span><span class="sxs-lookup"><span data-stu-id="25c0d-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="25c0d-110">**כתובת דואר אלקטרוני של** שולח : כתובת דואר אלקטרוני של שולח יחיד.</span><span class="sxs-lookup"><span data-stu-id="25c0d-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="25c0d-111">**כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.</span><span class="sxs-lookup"><span data-stu-id="25c0d-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="25c0d-112">**נושא**: השתמש בנושא כולו של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="25c0d-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="25c0d-113">החיפוש אינו תלוי רישיות.</span><span class="sxs-lookup"><span data-stu-id="25c0d-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="25c0d-114">לאחר הזנת קריטריוני החיפוש, לחץ על רענן לחצן ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **רענן כדי לסנן** את התוצאות.</span><span class="sxs-lookup"><span data-stu-id="25c0d-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="25c0d-115">כלי ה- cmdlet השתמשו כדי להציג ולנהל הודעות וקבצים בהסגר הם:</span><span class="sxs-lookup"><span data-stu-id="25c0d-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="25c0d-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="25c0d-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="25c0d-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="25c0d-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="25c0d-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="25c0d-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="25c0d-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): שים לב ש- cmdlet זה הוא רק עבור הודעות, ולא קבצי תוכנות זדוניות מ- Microsoft Defender עבור Office 365 עבור SharePoint Online, OneDrive for Business או Teams.</span><span class="sxs-lookup"><span data-stu-id="25c0d-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="25c0d-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="25c0d-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)