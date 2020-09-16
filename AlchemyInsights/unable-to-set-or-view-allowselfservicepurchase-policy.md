---
title: לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735200"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase

בעת ניסיון להגדיר או להציג את מדיניות AllowSelfServicePurchase, אתה מקבל את הודעת השגיאה הבאה:

*HandleError: לא היתה אפשרות לאחזר מדיניות מוצר עם PolicyId ' AllowSelfServicePurchase ', ErrorMessage-החיבור המשמש כבסיס נסגר: אירעה שגיאה בלתי צפויה בשליחה.*

ייתכן שהסיבה לכך היא גירסה ישנה יותר של אבטחה בשכבת התעבורה (TLS). כדי לחבר את שירות MSCommerce, עליך להשתמש ב-TLS 1.2 או בגדול יותר.  

נסה את השלבים הבאים כדי להפעיל/להגדיר את פרוטוקול TLS ל-1.2, לאמת ולנסות שוב.
 1. בשורת הפקודה של PowerShell (PS C: \) הזן את הפקודה הבאה כדי להגדיר את הפרוטוקול TLS לגירסה 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. ודא שהפרוטוקולים של TLS נמצאים בשימוש, באמצעות הפקודה הבאה:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. נסה שוב לבצע את הפקודות קבל או עדכן לפי הצורך.

