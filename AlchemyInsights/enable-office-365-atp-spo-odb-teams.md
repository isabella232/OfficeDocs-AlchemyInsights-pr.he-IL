---
title: אפשר ATP Office 365 עבור SharePoint, OneDrive ו- Microsoft צוותים
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030982"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>אפשר Office 365 איום מתקדם הגנה עבור SharePoint במצב מקוון, OneDrive ו- Microsoft צוותים

1. עבור אל https://protection.office.com ולהיכנס.
2. בחר **ניהול איום** > **מדיניות** > **מסמכים מצורפים בטוחים**.
3. בחר **להפעיל ATP עבור SharePoint, OneDrive, ו- Microsoft צוותים**ולאחר מכן לחץ על **שמור**.
4. (מומלץ) מנהל כללי או כמנהל SharePoint Online, להפעיל cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם הפרמטר **DisallowInfectedFileDownload** מוגדר כ- *true*.
5. (מומלץ) [הגדר התראות](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) עבור הקבצים שאותרו.

> [!NOTE]
> ATP יבצע סריקה nto כל קובץ בודד ב- SharePoint Online, OneDrive או צוותים של Microsoft. קבצים נסרקים באופן אסינכרוני, באמצעות תהליך העושה שימוש שיתוף מוזמנים פעילות ואירועי, יחד עם בהיריסטיקה חכמים ואת אותות איום כדי לזהות קבצים מזיקים. ראה [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).