---
title: 726 חסימת העברת דואר אלקטרוני
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059633"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>חסימה או ביטול חסימה של העברת דואר אלקטרוני

כדי להפוך העברת דואר אלקטרוני לזמינה או ללא זמינה עבור תיבת דואר ספציפית, ראה [קביעת תצורה של העברת דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

ברמת הדייר, השליטה ב העברה חיצונית ת בוצע באמצעות מדיניות דואר זבל יוצא. באפשרותך לבדוק את מדיניות מסנן דואר הזבל היוצא [](https://protection.office.com/antispam) ממרכז האבטחה והתאימות כאן או באמצעות [הפקודה Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

אם אתה מקבל את השגיאה הבאה: **"550 5.7.520 Access נדחתה,** הארגון שלך אינו מאפשר העברה חיצונית" , ודא שתצורת המדיניות מוגדרת לאפשר העברה אוטומטית חיצונית.

**הערה:** מומלץ להפוך את מדיניות מסנן דואר הזבל היוצא לזמינה כברירת מחדל כדי להפוך אותה לזמינה רק עבור המשתמשים שתצטרך לבצע העברה חיצונית על-ידי יצירת מדיניות מותאמת אישית עבור משתמשים אלה. באפשרותך לקרוא עוד בהגדרה [של העברת דואר אלקטרוני חיצונית ב- Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).