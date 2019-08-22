---
title: קוד שגיאה 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), לשקול לאפשר ADAL על-ידי עריכת הרישום.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526999"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>אירעה שגיאה בעת הפעלת Office 2013 על שירותי שולחן עבודה מרוחק

אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), לשקול לאפשר ADAL על-ידי עריכת הרישום.
  
|**מפתח רישום**|**סוג**|**ערך**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

לקבלת מידע נוסף, ראה [הפעלת אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL זמינה כברירת מחדל ב- Office 365 ProPlus ו- Office 2016. שירותי שולחן עבודה מרוחק (RDS) היה שם קודם לכן שירותי מסופים.
  