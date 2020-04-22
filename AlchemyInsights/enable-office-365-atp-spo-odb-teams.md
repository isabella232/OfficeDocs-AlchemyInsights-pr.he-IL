---
title: אפשר ל-Office 365 ATP עבור SharePoint, OneDrive וצוותי Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703427"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>אפשר ל-Office 365 להגן על איום מתקדם עבור SharePoint Online, OneDrive וצוותי Microsoft

1. . היכנס https://protection.office.com והיכנס
2. בחר > **במדיניות** >  **ניהול האיומים****קבצים מצורפים בטוחים**.
3. בחר **באפשרות הפעל את ה-ATP לצוותי SharePoint, OneDrive ו-Microsoft**ולאחר מכן לחץ על **שמור**.
4. ומלץ כמנהל כללי או כמנהל מערכת של SharePoint Online, הפעל את יישומון ה [-Cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם **הפרמטר** מוגדר כ- *true*.
5. ומלץ [הגדיר התראות](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) עבור קבצים שזוהו.

> [!NOTE]
> ATP יסרוק לסרוק כל קובץ בודד ב-SharePoint Online, OneDrive או בצוותי Microsoft. הקבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועים של שיתוף ופעילות אורח, יחד עם היוריסטיקה חכמה ואותות איום כדי לזהות קבצים זדוניים. ראה [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).