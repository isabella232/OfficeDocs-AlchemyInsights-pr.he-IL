---
title: קוד שגיאה 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות שירותי שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינים על-ידי עריכת הרישום.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100763"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>שגיאה בעת הפעלת Office 2013 ב'שירותי שולחן עבודה מרוחק'

אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות שירותי שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינים על-ידי עריכת הרישום.
  
|**מפתח רישום**|**סוג**|**ערך**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

לקבלת מידע נוסף, ראה [הפיכת אימות מודרני לזמין עבור Office 2013 במכשירי Windows אחרים](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL זמין כברירת מחדל ב- יישומי Microsoft 365 לארגונים ו- Office 2016. בעבר נקראה שירותי שולחן עבודה מרוחק (RDS).
  