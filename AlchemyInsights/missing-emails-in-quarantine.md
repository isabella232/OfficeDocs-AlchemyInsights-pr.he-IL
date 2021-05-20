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
# <a name="missing-emails-in-quarantine"></a>הודעות דואר אלקטרוני חסרות בהסגר"

מנהלי מערכת יכולים [להציג, לשחרר או למחוק הודעות אלה.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

כדי לפתוח את מרכז & האבטחה, עבור אל [https://protection.office.com](https://protection.office.com/) . כדי לפתוח את דף ההסגר ישירות, עבור אל [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

באפשרותך לחפש לפי הערכים הבאים:  

- **מזהה הודעה:** המזהה הייחודי הכללי של ההודעה. אם תבחר הודעה ברשימה, הערך  **'מזהה הודעה'**  יופיע בחלונית  **הפרטים נשלף**  שמופיעה. מנהלי מערכת יכולים להשתמש [במעקב אחר](/microsoft-365/security/office-365-security/message-trace-scc) הודעות כדי למצוא הודעות ואת ערכי מזהה ההודעה המתאימים שלהם.
- **כתובת דואר אלקטרוני של** שולח : כתובת דואר אלקטרוני של שולח יחיד.
- **כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.
- **נושא**: השתמש בנושא כולו של ההודעה. החיפוש אינו תלוי רישיות.

לאחר הזנת קריטריוני החיפוש, לחץ על רענן לחצן ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **רענן כדי לסנן** את התוצאות.

כלי ה- cmdlet השתמשו כדי להציג ולנהל הודעות וקבצים בהסגר הם:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): שים לב ש- cmdlet זה הוא רק עבור הודעות, ולא קבצי תוכנות זדוניות מ- Microsoft Defender עבור Office 365 עבור SharePoint Online, OneDrive for Business או Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)