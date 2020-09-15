---
title: הפיכת Office 365 ATP לזמין עבור SharePoint, OneDrive ו-Microsoft Teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709908"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>הפעלת הגנת האיום המתקדמת של Office 365 עבור SharePoint Online, OneDrive ו-Microsoft Teams

1. עבור אל https://protection.office.com והיכנס.
2. בחר **Threat management**  >  **Policy**  >  **קבצים מצורפים בטוחים במדיניות**ניהול האיום.
3. בחר **הפעל את ATP עבור SharePoint, OneDrive ו-Microsoft teams**ולאחר מכן לחץ על **שמור**.
4. מומלץ כמנהל מערכת כללי או כמנהל מערכת של SharePoint Online, הגדר את ה [-Cmdlet set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) כאשר הפרמטר **DisallowInfectedFileDownload** מוגדר ל- *true*.
5. מומלץ [הגדרת התראות](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) עבור קבצים שזוהו.

> [!NOTE]
> ATP יופיע כדי לסרוק כל קובץ בודד ב-SharePoint Online, ב-OneDrive או ב-Microsoft Teams. הקבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועים של שיתוף ופעילויות אורח, יחד עם היישויות חכמות ואותות איום כדי לזהות קבצים זדוניים. ראה [ATP עבור SharePoint, OneDrive ו-Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).