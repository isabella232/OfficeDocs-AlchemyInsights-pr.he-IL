---
title: פתח באמצעות הסייר אינו פועל
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906805"
---
# <a name="open-with-explorer-isnt-working"></a>פתח באמצעות הסייר אינו פועל

אם **פתח באמצעות סייר** או **תצוגה ב- Explorer קובץ** אינה פועלת ודא כי שירות WebClient מוגדר **פועל** על-ידי ביצוע השלבים הבאים. לדוגמה, היא עשויה להימשך זמן רב כדי לפתוח ספריית SharePoint או OneDrive כאשר השירות אינו פועל. 
  
1. בתיבת החיפוש של Windows, סוג הפעלה, בחר את הפעל app שולחן העבודה, סוג services. msc ולאחר מכן בחר **Enter**.
    
2. גלול מטה אל שירות WebClient ובדוק את עמודה **מצב** . אם המצב שירות WebClient אינו **פועל**, לחץ פעמיים על השירות, לחץ על **התחל**ולאחר מכן לחץ על **אישור**. הפעל את השירות, במידת הצורך, על-ידי בחירה **ידנית** או **אוטומטית** בתיבה **סוג הפעלה** . 
    
> [!NOTE]
> כדי לפתור בעיות בפתיחת בסייר קבצים, ראה [פתיחה בסייר](https://go.microsoft.com/fwlink/?linkid=871665). סיור סינכרון בתור חלופה טובה יותר: [SharePoint סינכרון קבצים עם לקוח סינכרון OneDrive החדש](https://go.microsoft.com/fwlink/?linkid=871666). 
  

