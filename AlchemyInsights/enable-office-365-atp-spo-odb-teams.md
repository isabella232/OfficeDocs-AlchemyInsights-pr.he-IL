---
title: הפיכת Office 365 ATP לזמין עבור SharePoint, OneDrive ו- Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896604"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>הפיכת Microsoft Defender לזמין Office 365 עבור SharePoint מקוון, OneDrive ו- Microsoft Teams

1. עבור https://protection.office.com אל והירשם.
2. בחר **מדיניות ניהול**  >  **איומים**  >  **כספת קבצים מצורפים**.
3. בחר **הפעל את Defender עבור Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams** ולאחר מכן לחץ על **שמור**.
4. (מומלץ) כמנהל מערכת כללי או כמנהל מערכת SharePoint Online, הפעל [את ה- cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם **הפרמטר DisallowInfectedFileDownload** מוגדר ל- *true*.
5. (מומלץ) [הגדר התראות עבור](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) קבצים שזוהו.

> [!NOTE]
> Microsoft Defender עבור Office 365 לא יסרוק כל קובץ ב- SharePoint Online, OneDrive או Microsoft Teams. קבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועי שיתוף ופעילות אורח, יחד עם הוריסטיקות חכמות ואותות איום לזיהוי קבצים זדוניים. עיין [ב- Microsoft Defender לקבלת Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)