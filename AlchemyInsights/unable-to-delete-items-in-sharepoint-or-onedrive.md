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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571258"
---
# <a name="unable-to-delete-items"></a>אין אפשרות למחוק פריטים

מדיניות שמירה עלולה לגרום לכך, עליך לבטל או להוציא החזקה בהתאמה שגורמת לבעיה זו. לאחר הסרת מדיניות שמירה או החזקה, ייתכן שהשינוי ישפיע עד 24 שעות. ודא שלא קיימת הגדרת [מדיניות שמירה](https://docs.microsoft.com/office365/securitycompliance/retention-policies) בפריט.

ייתכן שהאתר חרג ממגבלת האחסון, הגדל את [מיכסת האתר](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ומחק את הפריט.

ודא שהפריט לא [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.

לבסוף, מנהלי מערכת יכולים להשתמש [בתבניות ובשיטות](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) עבודה של SharePoint (PnP) המכילים ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות כגון כפיית מחיקת פריטים עקשנים.
- [הסר קובץ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [הסר תיקיית PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [הסר פריט רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [הסר רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [הסר שדה PNP (עמודה)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)