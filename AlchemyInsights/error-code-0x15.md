---
title: קוד שגיאה 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: אם אתה מקבל שגיאה בעת הפעלת הפריסה של Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506847"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>שגיאה בעת הפעלת Office 2013 בשירותי שולחן עבודה מרוחק

אם אתה מקבל שגיאה בעת הפעלת הפריסה של Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.
  
|**מפתח רישום**|**סוג**|**ערך**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

לקבלת מידע נוסף, ראה [הפיכת אימות מודרני לזמין עבור Office 2013 בהתקני Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL מופעלת כברירת מחדל ב-Microsoft 365 Apps עבור הארגון ו-Office 2016. שירותי שולחן עבודה מרוחק (RDS) נקראו בעבר שירותי מסופים.
  