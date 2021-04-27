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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059816"
---
# <a name="troubleshooting-pst-import-issues"></a>פתרון בעיות ייבוא PST

- אם אתה מייבא בתוך לקוח Outlook עצמו, ראה [פתרון בעיות בייבוא קובץ .pst של Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- אם אתה משתמש בשירות ייבוא והוא תקוע, שים לב שכל קובץ PST שאתה מעלה למיקום Azure Storage לא אמור להיות גדול מ- 20GB. קבצי PST הגדולים מ- 20GB עשויים להשפיע על הביצועים של תהליך הייבוא של PST. לקבלת מידע נוסף פתרון בעיות של משימות תקועות, ראה בעיות [המשפיעות על משימות ייבוא PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- אם ברצונך לאמת את המצב של משימת ייבוא ספציפית, השתמש [ב- Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- לקבלת פרטים מלאים על שירות הייבוא, ראה [מבט כולל על ייבוא קבצי ה- PST של הארגון שלך.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
