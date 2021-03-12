---
title: הפיכת Microsoft Defender לזמין עבור Office 365 עבור SharePoint Online, OneDrive ו-Microsoft Teams
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745305"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>הפיכת Microsoft Defender לזמין עבור Office 365 עבור SharePoint Online, OneDrive ו-Microsoft Teams

1. באמצעות אישורי מנהל המערכת הכלליים או מנהל האבטחה שלך, היכנס [למרכז האבטחה והתאימות של Office 365](https://protection.office.com/).
2. בחר **ניהול סיכונים** בחלונית הימנית ולאחר מכן בחר באפשרות קבצים מצורפים בטוחים **של מדיניות**  >  [](https://protection.office.com/safeattachment).
3. בחר **הפעל את Microsoft Defender עבור Office 365 עבור SharePoint, OneDrive ו-Microsoft teams** ולאחר מכן בחר **שמור**.
    > [!TIP]
    >
    > - כמנהל מערכת כללי או כמנהל מערכת של SharePoint Online, הגדר את ה-cmdlet הבא של PowerShell כאשר הפרמטר **DisallowInfectedFileDownload** מוגדר ל- *true*: [set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [הגדרת התראות עבור קבצים שזוהו](https://go.microsoft.com/fwlink/?linkid=2092110)

לקבלת מידע נוסף, ראה [Microsoft Defender עבור Office 365 עבור SharePoint, OneDrive ו-Microsoft teams](https://go.microsoft.com/fwlink/?linkid=2092041).
