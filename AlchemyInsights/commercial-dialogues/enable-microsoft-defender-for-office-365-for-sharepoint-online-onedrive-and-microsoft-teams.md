---
title: הפיכת כספת קבצים מצורפים SharePoint באופן מקוון, OneDrive וקבצים Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894464"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>הפיכת כספת קבצים מצורפים SharePoint באופן מקוון, OneDrive וקבצים Microsoft Teams

1. באמצעות אישורי מנהל המערכת הכללי או מנהל האבטחה שלך, פתח את פורטל Microsoft 365 Defender ב- ולאחר מכן עבור אל <https://security.microsoft.com> **מדיניות & כללי** מדיניות \>  \> **של איומים כספת קבצים מצורפים** **במקטע מדיניות**

   כדי לעבור ישירות לדף **כספת קבצים מצורפים,** השתמש <https://security.microsoft.com/safeattachmentv2> ב- .

2. בדף כספת **קבצים מצורפים,** לחץ על **הגדרות כלליות.**
3. בתפריט נשלף שמופיע, בחר הפעל את Microsoft Defender עבור Office 365 עבור **SharePoint, OneDrive ו- Microsoft Teams** ולאחר מכן בחר **שמור**.

    > [!TIP]
    >
    > בצע את השלבים הבאים כדי לשפר את ההגנה כספת קבצים מצורפים עבור SharePoint, OneDrive וקבצים Microsoft Teams:
    >
    > - כדי למנוע ממשתמשים להוריד קבצים זדוניים, השתמש בערך עבור `$true` *הפרמטר DisallowInfectedFileDownload* **[ב- cmdlet Set-SPOTenant ב-](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** SharePoint PowerShell מקוון. לקבלת מידע נוסף, [ראה שימוש SharePoint PowerShell מקוון כדי למנוע ממשתמשים להוריד קבצים זדוניים](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    > - [יצירת מדיניות התראה עבור קבצים שזוהו](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

לקבלת מידע נוסף, [ראה כספת קבצים מצורפים עבור Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
