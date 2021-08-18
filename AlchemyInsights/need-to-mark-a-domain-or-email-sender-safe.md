---
title: האם עליך לסמן תחום או שולח דואר אלקטרוני בטוחים?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319949"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>האם עליך לסמן תחום או שולח דואר אלקטרוני בטוחים?

- השימוש **ברשימות שולחים בטוחים אינו מומלץ מאחר** שהוא פותח את הארגון שלך כדי לשלוח הודעות זבל, דיוג ותקפות תוקף.
- עם זאת, אם יש דרישה עסקית, מומלץ **להשתמש** **[ב'דואר' Flow כללי](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** פעולה זו. ההנחיות שלנו מבטיחות אימות שולח (מוודאת שלא תפורסם שליחה של תחום). 
    **הערה:** איננו ממליצים לנהל תוצאות חיוביות שגויות באמצעות רשימות שולחים בטוחים, מכיוון שחסכון חריג לסינון דואר זבל יכול לפתוח את הארגון שלך להתקפות אבטחה. אם המשתמשים שלך מקבלים הודעות המסומנות באופן שגוי כדואר זבל או כדואר זבל, **[דווח על הודעות וקבצים ל- Microsoft.](https://protection.office.com/reportsubmission)**
- כספת יש להימנע משולחים Outlook, ברשימת שולחים מותרים או ברשימת תחומים מותרים במדיניות למניעת דואר זבל מכיוון ששולחים עוקפים את כל הודעות הדואר זבל, התחנפות וההגנה מפני דיוג ואימות שולח (SPF, DKIM, DMARC).  שיטה זו משמשת באופן הטוב ביותר לבדיקות זמניות בלבד.
- האימות שערכת דואר אלקטרוני מסוימת חלפה על-ידי בדיקת כותרת ההודעה "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKV:SKN), ראה כותרות הודעות למניעת דואר **[זבל.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- מאחר ש- Microsoft רוצה לשמור על אבטחת [הלקוחות שלנו כברירת מחדל,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)עקיפות דיירים מסוימים אינם מוחלים עבור תוכנות זדוניות ודיוג בביטחון גבוה. עקיפות אלה כוללות: o רשימות שולחים מותרים או רשימות תחומים מותרות (מדיניות למניעת דואר זבל) Outlook כספת שולחים או רשימת אפשרי IP (סינון חיבורים) 
- העקיפה היחידה המאפשרת לה הודעת דיוג בביטחון גבוה לעקוף את הסינון היא Exchange זרימת דואר (המכונה גם כללי תעבורה). כדי להשתמש בכללי זרימת דואר כדי לעקוף סינון, ראה שימוש בכללי זרימת דואר כדי להגדיר את רמת הביטחון של **[דואר זבל (SCL) בהודעות](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.