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
# <a name="missing-emails-in-quarantine"></a>הודעות דואר אלקטרוני חסרות בהסגר"

מנהלי מערכת יכולים [להציג, לשחרר או למחוק הודעות אלה.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

כדי לפתוח את מרכז & האבטחה, עבור אל [https://protection.office.com](https://protection.office.com/) . כדי לפתוח את דף ההסגר ישירות, עבור אל [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

באפשרותך לחפש לפי הערכים הבאים:  

- **מזהה הודעה:** המזהה הייחודי הכללי של ההודעה. אם תבחר הודעה ברשימה, הערך  **'מזהה הודעה'**  יופיע בחלונית  **הפרטים נשלף**  שמופיעה. מנהלי מערכת יכולים להשתמש [במעקב אחר](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) הודעות כדי למצוא הודעות ואת ערכי מזהה ההודעה המתאימים שלהם.
- **כתובת דואר אלקטרוני של** שולח : כתובת דואר אלקטרוני של שולח יחיד.
- **כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.
- **נושא**: השתמש בנושא כולו של ההודעה. החיפוש אינו תלוי רישיות.

לאחר הזנת קריטריוני החיפוש, לחץ על רענן לחצן ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **רענן כדי לסנן** את התוצאות.  

כלי ה- cmdlet השתמשו כדי להציג ולנהל הודעות וקבצים בהסגר הם:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש- cmdlet זה הוא רק עבור הודעות, ולא קבצי תוכנה זדונית מ- ATP עבור SharePoint Online, OneDrive for Business או Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)