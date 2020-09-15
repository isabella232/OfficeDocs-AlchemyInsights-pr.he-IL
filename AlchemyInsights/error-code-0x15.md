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
description: אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותים של שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709188"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>שגיאה בעת הפעלת Office 2013 בשירותי שולחן עבודה מרוחק

אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותים של שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.
  
|**מפתח רישום**|**סוג**|**ערך**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

לקבלת מידע נוסף, ראה [הפיכת אימות מודרני לזמין עבור Office 2013 במכשירי Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL מופעל כברירת מחדל באפליקציות Microsoft 365 עבור enterprise ו-Office 2016. שירותי שולחן עבודה מרוחק (RDS) נקראו בעבר ' שירותי מסופים '.
  