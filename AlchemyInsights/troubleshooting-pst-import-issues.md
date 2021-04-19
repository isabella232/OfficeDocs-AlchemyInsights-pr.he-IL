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
# <a name="troubleshooting-pst-import-issues"></a>פתרון בעיות ייבוא PST

- אם אתה מייבא בתוך לקוח Outlook עצמו, ראה [פתרון בעיות בייבוא קובץ. pst של Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- אם אתה משתמש בשירות הייבוא והוא נתקע, שים לב שכל קובץ PST שאתה מעלה למיקום באחסון Azure צריך להיות גדול מ- 20 GB. קבצי PST גדולים מ- 20 GB עלולים להשפיע על הביצועים של תהליך ייבוא PST.

- אם ברצונך לאמת את המצב של משימת ייבוא מסוימת, באפשרותך להשתמש ב[Get-MailboxImportRequest](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- לקבל פרטים מלאים אודות שירות הייבוא, ראה [סקירה של יבוא קבצי PST של הארגון שלך](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
