---
title: פתרון בעיות ייבוא PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826164"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="3914e-102">פתרון בעיות ייבוא PST</span><span class="sxs-lookup"><span data-stu-id="3914e-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="3914e-103">אם אתה מייבא בתוך לקוח Outlook עצמו, ראה [פתרון בעיות בייבוא קובץ. pst של Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="3914e-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="3914e-104">אם אתה משתמש בשירות הייבוא והוא נתקע, שים לב שכל קובץ PST שאתה מעלה למיקום באחסון Azure צריך להיות גדול מ- 20 GB.</span><span class="sxs-lookup"><span data-stu-id="3914e-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="3914e-105">קבצי PST גדולים מ- 20 GB עלולים להשפיע על הביצועים של תהליך ייבוא PST.</span><span class="sxs-lookup"><span data-stu-id="3914e-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="3914e-106">אם ברצונך לאמת את המצב של משימת ייבוא מסוימת, באפשרותך להשתמש ב[Get-MailboxImportRequest](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="3914e-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="3914e-107">לקבל פרטים מלאים אודות שירות הייבוא, ראה [סקירה של יבוא קבצי PST של הארגון שלך](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3914e-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
