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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892048"
---
# <a name="missing-emails-in-quarantine"></a>הודעות דואר אלקטרוני חסרות בהסגר

מנהלי מערכת יכולים [להציג, לשחרר או למחוק הודעות אלה](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל סקירת **ההסגר.** \>  לחלופין, כדי לעבור ישירות לדף **ההסגר,** השתמש <https://security.microsoft.com/quarantine> ב- .  

לקבלת מידע נוסף אודות ערכי החיפוש/הסינון בהם באפשרותך להשתמש, ראה ניהול הודעות וקבצים [בהסגר כמנהל מערכת ב- EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

כלי ה- cmdlet השתמשו בהם כדי להציג ולנהל הודעות וקבצים בהסגר הם:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): שים לב ש- cmdlet זה הוא רק עבור הודעות, לא קבצים מ- כספת קבצים מצורפים עבור SharePoint, OneDrive או Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
