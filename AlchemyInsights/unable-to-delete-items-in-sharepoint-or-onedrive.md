---
title: אין אפשרות למחוק פריטים ב-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511977"
---
# <a name="unable-to-delete-items"></a>אין אפשרות למחוק פריטים

מדיניות שמירה עלולה לגרום לכך, עליך לבטל או להוציא החזקה בהתאמה שגורמת לבעיה זו. לאחר הסרת מדיניות שמירה או החזקה, ייתכן שהשינוי ישפיע עד 24 שעות. ודא שלא קיימת הגדרת [מדיניות שמירה](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) בפריט.

ייתכן שהאתר חרג ממגבלת האחסון, הגדל את [מיכסת האתר](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ומחק את הפריט.

ודא שהפריט לא [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.

לבסוף, מנהלי מערכת יכולים להשתמש [בתבניות ובשיטות](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) עבודה של SharePoint (PnP) המכילים ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות כגון כפיית מחיקת פריטים עקשנים.
- [הסר קובץ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [הסר תיקיית PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [הסר פריט רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [הסר רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [הסר שדה PNP (עמודה)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)