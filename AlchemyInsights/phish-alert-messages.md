---
title: 2491 הודעות דואר אלקטרוני של התראה ממדיניות 'דיוג נמסר עקב דייר או עקיפת משתמש'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316359"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>התראת הודעות דואר אלקטרוני ממדיניות 'דיוג נמסר עקב דייר או עקיפת משתמש'

מדיניות התראה המוגדרת כברירת מחדל בשם **דיוג** נמסרה עקב דייר או עקיפת משתמש זמינה בארגונים עם Microsoft Defender עבור Office 365 P1 ורשיון P2. אם קיבלת התראה זו, להלן השלבים לתחקור:

1. מתוך הודעת ההתראה, **לחץ על הצג** התראה כדי לעבור **לדף** התראות בפורטל Microsoft 365 Defender.

2. בחר את ההתראה כדי לראות את האפשרות להציג **רשימת הודעות או** **להציג הודעות בסייר**. שתי אפשרויות אלה לוקחות אותך לפרטי ההודעה, הכוללת את מזהה ההודעה. שים לב שהקישור 'סייר איומים' ילסנן באופן אוטומטי את ההודעות התואמות לקריטריוני ההתראה. ייתכן שיהיה עליך להתאים את מסנן התאריך בסייר האיומים.

הודעת דיוג נמסרה עקב עקיפה שתצורתה נקבעה באופן ידני:

- שולח או תחום מותרים המוגדרים על-ידי המשתמש.
- שולח או תחום מותרים המוגדרים על-ידי מנהל המערכת במדיניות למניעת דואר זבל.
- כתובת IP מותרת במדיניות מסנן חיבור.
- כלל זרימת דואר (הידוע גם ככלל תעבורה) שתצורתו נקבעה לאפשר הודעות.

אם אתה סבור שההודעה סומנה באופן שגוי כ דיוג, השתמש [בשליחה](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) של מנהל מערכת כדי הדוח את ההודעה ל- Microsoft.

משתמשים יכולים להשתמש [תוספת 'הודעת דוח' או](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) התוספת 'דיווח על דיוג' Outlook כדי לשלוח דוגמאות הודעה ל- Microsoft.
