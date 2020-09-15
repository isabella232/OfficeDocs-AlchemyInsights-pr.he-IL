---
title: האפשרות ' פתח באמצעות Explorer ' אינה פועלת
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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694457"
---
# <a name="open-with-explorer-isnt-working"></a>האפשרות ' פתח באמצעות Explorer ' אינה פועלת

אם **האפשרות פתח באמצעות סייר** או **תצוגה בסייר הקבצים** אינה פועלת, ודא ששירות WebClient מוגדר **לפעול** על-ידי ביצוע השלבים שלהלן. לדוגמה, ייתכן שיחלפו זמן רב לפתיחת ספריה של SharePoint או OneDrive כאשר השירות אינו פועל. 
  
1. בתיבת החיפוש של Windows, הקלד הופעל, בחר את יישום שולחן העבודה, הקלד services. msc ולאחר מכן בחר **Enter**.
    
2. גלול מטה אל שירות WebClient ובדוק את העמודה **מצב** . אם מצב השירות של WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**. הפוך את השירות לזמין, במידת הצורך, על-ידי בחירה באפשרות **ידני** או **אוטומטי** בתיבה **סוג הפעלה** . 
    
> [!NOTE]
> כדי לפתור בעיות שנפתחות בסייר הקבצים, ראה [פתח ב-explorer](https://go.microsoft.com/fwlink/?linkid=871665). גלה את הסינכרון כחלופה טובה יותר: [סנכרן קבצי SharePoint עם לקוח הסינכרון החדש של OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

