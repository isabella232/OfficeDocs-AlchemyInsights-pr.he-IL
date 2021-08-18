---
title: חסימה או ביטול חסימה של העברת דואר אלקטרוני אוטומטית חיצונית
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897469"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>חסימה או ביטול חסימה של העברת דואר אלקטרוני אוטומטית נצחית

כדי להפוך העברת דואר אלקטרוני לזמינה או ללא זמינה עבור תיבת דואר ספציפית, ראה [קביעת תצורה של העברת דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

מנהלי מערכת יכולים לשלוט בהעברות חיצוניות עבור הארגון [באמצעות מדיניות דואר זבל יוצא.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) אתה מנהל מדיניות דואר זבל יוצא בפורטל Microsoft 365 Defender <https://security.microsoft.com/antispam> [ב- Get-HostedOutboundSpamFilterPolicy ב-](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Exchange Online PowerShell.

אם אתה מקבל את השגיאה הבאה: **"550 5.7.520 Access נדחית,** הארגון שלך אינו מאפשר העברה חיצונית" , ודא שהמדיניות מוגדרת לאפשר הודעות חיצוניות שהועברו באופן אוטומטי.

**הערה:** המלצנו על ערך ברירת  המחדל אוטומטי **-** מערכת מבוקרת עבור הגדרת כללי העברה אוטומטית במדיניות מסנן דואר הזבל היוצא המוגדר כברירת מחדל (העברה חיצונית אוטומטית חסומה; העברה אוטומטית פנימית עדיין פועלת). עליך ליצור פריטי מדיניות מותאמים אישית של מסנן דואר זבל יוצא ולהשתמש בערך **On - Forwarding** זמין רק עבור משתמשים שתצטרך העברת דואר אלקטרוני אוטומטית חיצונית. לקבלת מידע נוסף, ראה [קביעת תצורה של העברת דואר אלקטרוני חיצונית ב- Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
