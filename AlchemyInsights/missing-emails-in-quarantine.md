---
title: הודעות דואר אלקטרוני חסרות בהסגר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673715"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="954a8-102">הודעות דואר אלקטרוני חסרות בהסגר</span><span class="sxs-lookup"><span data-stu-id="954a8-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="954a8-103">מנהלי [מערכת יכולים להציג, לשחרר או למחוק הודעות אלה.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="954a8-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="954a8-104">כדי לפתוח את מרכז התאימות של אבטחה &, עבור אל [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="954a8-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="954a8-105">כדי לפתוח את דף ההסגר ישירות, עבור אל [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="954a8-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="954a8-106">באפשרותך לחפש לפי הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="954a8-106">You can search by the following values:</span></span>  

- <span data-ttu-id="954a8-107">**מזהה הודעה**: המזהה הייחודי הכללי של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="954a8-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="954a8-108">אם תבחר הודעה ברשימה, ערך  **מזהה ההודעה**  יופיע בחלונית  **פרטים**  נשלף של שמופיעה.</span><span class="sxs-lookup"><span data-stu-id="954a8-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="954a8-109">מנהלי מערכת יכולים להשתמש [במעקב אחר](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) הודעות כדי לחפש הודעות וערכי מזהה ההודעות המתאימים שלהם.</span><span class="sxs-lookup"><span data-stu-id="954a8-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="954a8-110">**כתובת הדואר האלקטרוני של השולח**: כתובת דואר אלקטרוני של שולח יחיד.</span><span class="sxs-lookup"><span data-stu-id="954a8-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="954a8-111">**כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.</span><span class="sxs-lookup"><span data-stu-id="954a8-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="954a8-112">**נושא**: השתמש בנושא כולו של ההודעה.</span><span class="sxs-lookup"><span data-stu-id="954a8-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="954a8-113">החיפוש אינו תלוי רישיות.</span><span class="sxs-lookup"><span data-stu-id="954a8-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="954a8-114">לאחר שהזנת את קריטריוני החיפוש, לחץ על רענון ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** לחצן רענן כדי לסנן את התוצאות.  </span><span class="sxs-lookup"><span data-stu-id="954a8-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="954a8-115">רכיבי ה-cmdlet שבהם אתה משתמש כדי להציג ולנהל הודעות וקבצים בהסגר הם:</span><span class="sxs-lookup"><span data-stu-id="954a8-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="954a8-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="954a8-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="954a8-117">ייצוא-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="954a8-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="954a8-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="954a8-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="954a8-119">[תצוגה מקדימה-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש-cmdlet זה מיועד רק להודעות, ולא לקבצי תוכנות זדוניות מ-ATP עבור SharePoint Online, OneDrive for Business או teams.</span><span class="sxs-lookup"><span data-stu-id="954a8-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="954a8-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="954a8-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)