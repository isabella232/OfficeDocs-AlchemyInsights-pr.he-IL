---
title: לא ניתן למחוק פריטים SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038518"
---
# <a name="unable-to-delete-items"></a>לא ניתן למחוק פריטים

- מדיניות שמירה עשויה לגרום לכך, עליך להפוך את החסימת החסימת המתאימה ללא זמינה או לא לכלול אותה גורמת לבעיה זו. לאחר הסרת מדיניות שמירה או החזקה, ייתכן שהשינוי יתוקף עד 24 שעות. ודא שאין הגדרת [מדיניות שמירה](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) בפריט.

- ייתכן שהמקום חרג ממגבלת האחסון, להגדיל את [מיכסת האתר](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ולמחוק את הפריט.

- ודא שהפריט [לא יצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.

- לבסוף, מנהלי מערכת יכולים [להשתמש ב- SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) דפוסים ותרגולים (PnP) המכילה ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות, כגון כפיית מחיקת פריטים עקשניים.
- [הסרת קובץ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [הסרת תיקיית PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [הסרת פריט רשימה של PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [הסרת רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [הסרת שדה PNP (עמודה)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)