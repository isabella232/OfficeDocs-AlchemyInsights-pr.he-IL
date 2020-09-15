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
# <a name="missing-emails-in-quarantine"></a>הודעות דואר אלקטרוני חסרות בהסגר

מנהלי [מערכת יכולים להציג, לשחרר או למחוק הודעות אלה.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

כדי לפתוח את מרכז התאימות של אבטחה &, עבור אל [https://protection.office.com](https://protection.office.com/) . כדי לפתוח את דף ההסגר ישירות, עבור אל [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

באפשרותך לחפש לפי הערכים הבאים:  

- **מזהה הודעה**: המזהה הייחודי הכללי של ההודעה. אם תבחר הודעה ברשימה, ערך  **מזהה ההודעה**  יופיע בחלונית  **פרטים**  נשלף של שמופיעה. מנהלי מערכת יכולים להשתמש [במעקב אחר](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) הודעות כדי לחפש הודעות וערכי מזהה ההודעות המתאימים שלהם.
- **כתובת הדואר האלקטרוני של השולח**: כתובת דואר אלקטרוני של שולח יחיד.
- **כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.
- **נושא**: השתמש בנושא כולו של ההודעה. החיפוש אינו תלוי רישיות.

לאחר שהזנת את קריטריוני החיפוש, לחץ על רענון ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** לחצן רענן כדי לסנן את התוצאות.  

רכיבי ה-cmdlet שבהם אתה משתמש כדי להציג ולנהל הודעות וקבצים בהסגר הם:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [ייצוא-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [תצוגה מקדימה-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש-cmdlet זה מיועד רק להודעות, ולא לקבצי תוכנות זדוניות מ-ATP עבור SharePoint Online, OneDrive for Business או teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)