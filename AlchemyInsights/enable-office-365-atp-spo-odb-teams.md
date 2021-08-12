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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964634"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>הפוך את Microsoft Defender לזמין Office 365 עבור SharePoint מקוון, OneDrive ו- Microsoft Teams

1. עבור https://protection.office.com אל והירשם.
2. בחר **מדיניות ניהול**  >  **איומים**  >  **כספת קבצים מצורפים**.
3. בחר **הפעל את Defender עבור Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams** ולאחר מכן לחץ על **שמור**.
4. (מומלץ) כמנהל מערכת כללי או כמנהל מערכת SharePoint Online, הפעל [את cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם **הפרמטר DisallowInfectedFileDownload** מוגדר ל- *true*.
5. (מומלץ) [הגדר התראות עבור](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) קבצים שזוהו.

> [!NOTE]
> Microsoft Defender עבור Office 365 לא יסרוק כל קובץ ב- SharePoint Online, OneDrive או Microsoft Teams. קבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועי שיתוף ופעילות אורח, יחד עם הוריסטיקות חכמות ואותות איומים לזיהוי קבצים זדוניים. עיין [ב- Microsoft Defender לקבלת Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)