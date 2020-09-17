---
title: אין אפשרות למחוק פריטים ב-SharePoint או ב-OneDrive
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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806112"
---
# <a name="unable-to-delete-items"></a>לא ניתן למחוק פריטים

מדיניות שמירה יכולה לגרום לכך, עליך להפוך ללא זמין או לא לכלול החזקה שגורמת לבעיה זו. לאחר הסרת מדיניות שמירה או חסימה, ייתכן שיחלפו עד 24 שעות כדי שהשינוי ייכנס לתוקף. ודא שאין הגדרת [מדיניות שמירה](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) על הפריט.

ייתכן שהאתר חרג ממגבלת האחסון, הגדל את [מיכסת האתר](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ומחק את הפריט.

ודא שהפריט לא [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.

בסופו של דבר, מנהלי מערכת יכולים להשתמש [בתבניות ובתרגולים של SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) אשר מכילים ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות כגון כפה על מחיקת פריטים עקשניים.
- [הסרת קובץ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [הסרת תיקיית PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [הסרת פריט רשימה של PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [הסרת רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [הסרת שדה PNP (עמודה)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)