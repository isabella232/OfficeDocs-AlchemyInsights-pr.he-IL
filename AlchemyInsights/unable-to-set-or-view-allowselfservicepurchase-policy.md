---
title: לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826092"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase

בעת ניסיון להגדיר או להציג את מדיניות AllowSelfServicePurchase, מתקבלת הודעת השגיאה הבאה:

*HandleError : לא היתה אפשרות לאחזר מדיניות מוצר באמצעות PolicyId 'AllowSelfServicePurchase', ErrorMessage - החיבור שמשמש בסיס נסגר: אירעה שגיאה בלתי צפויה בשליחה.*

ייתכן שהגורם הוא גירסה קודמת של אבטחת שכבת תעבורה (TLS). כדי לחבר את שירות MSCommerce, עליך להשתמש ב- TLS 1.2 לחלופין.  

נסה את השלבים הבאים כדי להפעיל/להגדיר את פרוטוקול TLS ל- 1.2, לאמת ונסה שוב.
 1. בשורת הפקודה של PowerShell (PS C: \) הזן את הפקודה הבאה כדי להגדיר את פרוטוקול TLS לגירסה 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. אמת את הפרוטוקולים של TLS בשימוש, באמצעות הפקודה הבאה:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. נסה שוב את הפקודות קבל או עדכן כצורך.

