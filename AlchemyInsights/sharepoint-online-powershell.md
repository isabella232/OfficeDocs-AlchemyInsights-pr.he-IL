---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830583"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

עובד עם PowerShell או עם קבצי Script בתוך Sharepoint Online? בקר בקישורים שלהלן לקבלת מידע נוסף.
- [תחילת העבודה עם מעטפת הניהול של SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [התחבר ל- SPO PowerShell באמצעות אימות רב-תכליתי (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) מכיל ספריה של פקודות PowerShell המאפשרת לך לבצע פעולות ניהול מורכבות כלפי SPO.

> [!NOTE]
> - אם אתה נתקל בבעיות בהתחברות עם מעטפת ניהול ה- SPO, ודא כי עדכנת את הגירסה העדכנית ביותר ונסה לייבא מחדש את [המודול](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) באמצעות *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - אם אתה מנסה להפעיל קבצי Script של מודל אובייקט בצד הלקוח, יהיה עליך להתקין [את ה- SDK של רכיבי לקוח של Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) במחשב המקומי שלך.
> - אם אתה נתקל בבעיות בהפעלת קבצי Script מ- PowerShell, ייתכן שתרצה לשקול להפעיל את PowerShell כמנהל מערכת ושינוי [מדיניות הביצוע](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).