---
title: הפתיחה באמצעות סייר אינה פועלת
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713035"
---
# <a name="open-with-explorer-isnt-working"></a>הפתיחה באמצעות סייר אינה פועלת

אם **הפתיחה באמצעות סייר** או **תצוגה ב-Explorer של הקובץ** אינה פועלת, ודא שהשירות webclient מוגדר **לפעולה** על-ידי ביצוע השלבים שלהלן. לדוגמה, ייתכן שייקח זמן רב לפתוח ספריית SharePoint או OneDrive כאשר השירות אינו פועל. 
  
1. בתיבת החיפוש של Windows, הקלד הפעלה, בחר את יישום שולחן העבודה, הקלד services. msc ולאחר מכן בחר באפשרות **Enter**.
    
2. גלול מטה לשירות WebClient ובדוק את עמודת **המצב** . אם מצב השירות WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**. הפעל את השירות, במידת הצורך, על-ידי בחירה באפשרות **ידני** או **אוטומטי** בתיבה **סוג הפעלה** . 
    
> [!NOTE]
> כדי לפתור בעיות פתיחה בסייר הקבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665). סקור את הסינכרון כחלופה טובה יותר: [סנכרן קבצי SharePoint עם לקוח הסינכרון החדש OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

