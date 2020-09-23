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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219856"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>חסימה או ביטול חסימה של העברת דואר אלקטרוני

כדי להפוך העברת דואר אלקטרוני לזמינה או ללא זמינה עבור תיבת דואר ספציפית, ראה [קביעת תצורה של העברת דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

ברמת הדיירים, השליטה על העברה חיצונית מתבצעת באמצעות המדיניות היוצאת למניעת דואר זבל. אם הוא מוגדר כבוטל או אוטומטי, ייתכן שהוא יחסום את העברת הדואר האלקטרוני באמצעות השגיאה "550 5.7.520 הגישה נדחתה, הארגון שלך אינו מאפשר העברה חיצונית". לאחר מכן, אם הוגדרה העברה שנחסמה, זוהי השגיאה שהמשתמשים יראו.

אם העברת העברה נחסמת, ודא שהמדיניות נקבעה להפיכת Autoforward חיצוניים לזמין. באפשרותך לבדוק את מדיניות המסנן ' דואר זבל יוצא ' ממרכז האבטחה והתאימות או על-ידי הפעלת Get-HostedOutboundSpamFilterPolicy | שם fl, AutoForwardingMode. אם ברצונך להגדיר חסימת Autoforward, אותה פקודה תספר לך את מצב המדיניות כעת.

הערה: מומלץ להשאיר את הAutoforward החיצוניים ללא זמין במדיניות מסנן דואר הזבל היוצא המהווה ברירת מחדל ולהפוך אותה לזמינה רק עבור המשתמשים הזקוקים להעברה חיצונית על-ידי יצירת מדיניות מותאמת אישית עבור משתמשים אלה. באפשרותך לקרוא עוד [בקביעת התצורה של העברת דואר אלקטרוני חיצוני ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).