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
# <a name="missing-emails-in-quarantine"></a>הודעות דוא ל חסרות בהסגר

מנהלי [מערכת יכולים להציג, לשחרר או למחוק הודעות אלה.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

כדי לפתוח את מרכז התאימות של אבטחה _ אמפר, עבור אל https://protection.office.com . כדי לפתוח את דף ההסגר ישירות, עבור אל https://protection.office.com/quarantine .  

באפשרותך לחפש לפי הערכים הבאים:  

- **מזהה הודעה**: המזהה הייחודי הגלובלי של ההודעה. אם תבחר הודעה ברשימה, ערך **מזהה ההודעה** יופיע בחלונית **הפרטים** הנפתחת שמופיעה. למנהלים יש אפשרות להשתמש [במעקב אחר](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) הודעות כדי לחפש את ההודעות ואת ערכי מזהה ההודעה המתאימים להם.
- **כתובת אימייל של השולח**: כתובת אימייל של שולח אחד.
- **כתובת דואר אלקטרוני של נמען**: כתובת דואר אלקטרוני של נמען יחיד.
- **נושא**: השתמש בנושא כולו של ההודעה. החיפוש אינו תלוי רישיות.

לאחר שהזנת את קריטריוני החיפוש, לחץ על ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **רענן** לחצן רענון כדי לסנן את התוצאות.  

יישומוני ה-cmdlet שבהם אתה משתמש כדי להציג ולנהל הודעות וקבצים בהסגר הם:
- [הודעת מחיקה-הודעה](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [הודעת ייצוא-בהסגר](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [הודעת ' קבל-בהסגר '](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- הודעת בכיוון [תצוגה מקדימה](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש-cmdlet זה מיועד רק להודעות, לא לקבצים של תוכנות זדוניות מ-ATP עבור SharePoint Online, Onedrive עבור עסקים או צוותים.
- [הודעת שחרור בהסגר](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)