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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329663"
---
# <a name="missing-emails-in-quarantine"></a>הודעות דואר אלקטרוני חסרות בהסגר

מנהלי מערכת יכולים [להציג, לשחרר או למחוק הודעות אלה](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל סקירת **ההסגר.** \>  לחלופין, כדי לעבור ישירות לדף **ההסגר,** השתמש <https://security.microsoft.com/quarantine> ב- .  

לקבלת מידע נוסף אודות ערכי החיפוש/הסינון בהם באפשרותך להשתמש, ראה ניהול הודעות וקבצים [בהסגר כמנהל מערכת ב- EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

כלי ה- cmdlet השתמשו בהם כדי להציג ולנהל הודעות וקבצים בהסגר הם:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש- cmdlet זה הוא רק עבור הודעות, ולא קבצים מ- כספת קבצים מצורפים עבור SharePoint, OneDrive או Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
