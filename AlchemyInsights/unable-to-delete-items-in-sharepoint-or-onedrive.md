---
title: אין אפשרות למחוק פריטים ב- SharePoint או OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757926"
---
# <a name="unable-to-delete-items"></a>אין אפשרות למחוק פריטים

נתקל בבעיות מחיקת פריטים?

- הקפד תמיד שיש לך את [ההרשאות המתאימות](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) כדי למחוק את הפריט או להיות בעל ניסיון [מנהל אוסף אתרים](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) להסיר את הפריט.

- ודא כי אין הגדרת [מדיניות שמירה](https://docs.microsoft.com/office365/securitycompliance/retention-policies) פריט.

- ודא שהפריט אינו [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) אל משתמש אחר.

- לבסוף, מנהלי מערכת יכולים להשתמש [תבניות SharePoint ותרגולים](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) אשר מכיל ספריה של PowerShell פקודות המאפשרות לך לבצע פעולות ניהול מורכבים כגון לכפות את מחיקת פריטים stubborn. 
- [הסרת קובץ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [הסרת תיקיה PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [הסר פריט רשימה PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [הסר את רשימת PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [הסרת PNP שדה (עמודה)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)