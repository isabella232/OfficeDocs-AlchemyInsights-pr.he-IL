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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478340"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>חסימה או ביטול חסימה של העברת דואר אלקטרוני

כדי להפוך העברת דואר אלקטרוני לזמינה או ללא זמינה עבור תיבת דואר ספציפית, ראה [קביעת תצורה של העברת דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

ברמת הדייר, השליטה על העברה חיצונית מתבצעת באמצעות מדיניות הדואר האלקטרוני היוצא. באפשרותך לבדוק את מדיניות המסנן של דואר זבל יוצא ממרכז האבטחה והתאימות [כאן](https://protection.office.com/antispam) או באמצעות [הפקודה Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

אם אתה מקבל את השגיאה הבאה: **"550 5.7.520 Access נדחה, הארגון שלך אינו מאפשר העברה חיצונית"**, ודא שהמדיניות מוגדרת להפיכת העברה אוטומטית אוטומטית לזמינה.

**הערה:** מומלץ למנוע מAutoforward החיצוניות להיות זמין במדיניות מסנן דואר הזבל היוצא המהווה ברירת מחדל, ולהפוך אותה לזמינה רק עבור המשתמשים הזקוקים להעברה חיצונית על-ידי יצירת מדיניות מותאמת אישית עבור משתמשים אלה. באפשרותך לקרוא עוד [בקביעת התצורה של העברת דואר אלקטרוני חיצוני ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).