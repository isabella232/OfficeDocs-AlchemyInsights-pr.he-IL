---
title: פתיחה באמצעות Explorer אינה פועלים
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011337"
---
# <a name="open-with-explorer-isnt-working"></a>פתח באמצעות Explorer אינו פועל

אם **פתח באמצעות סייר** או תצוגה **בסייר הקבצים** אינו פועל ודא ששירות WebClient מוגדר ל'פועל' **על-ידי** ביצוע השלבים הבאים. לדוגמה, ייתכן שתך זמן רב SharePoint ספריית OneDrive כאשר השירות אינו פועל. 
  
1. בתיבת Windows, הקלד run, בחר את האפליקציה הפעל שולחן עבודה, הקלד services.msc ולאחר מכן בחר **Enter**.
    
2. גלול מטה אל שירות WebClient ובדוק את **תיבת** הדו-שיח מצב עמודה. אם מצב השירות WebClient אינו **פועל, לחץ** פעמיים על השירות, לחץ על **התחל ולאחר** מכן לחץ על **אישור.** הפוך את השירות לזמין, לפי הצורך, **על-ידי** בחירה באפשרות ידני **או** אוטומטי **בתיבה סוג** אתחול. 
    
> [!NOTE]
> כדי לפתור בעיות בפתיחת סייר הקבצים, ראה [פתיחה בסייר.](https://go.microsoft.com/fwlink/?linkid=871665) סייר בסינכרון כ חלופה [טובה יותר: סינכרון SharePoint קבצים עם לקוח סינכרון OneDrive החדש](https://go.microsoft.com/fwlink/?linkid=871666). 
  

