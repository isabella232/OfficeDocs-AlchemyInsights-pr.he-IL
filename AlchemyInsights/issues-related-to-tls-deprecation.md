---
title: אין אפשרות לשלוח/לקבל דואר אלקטרוני אל/מ-Office 365 בשל היכולת של TLS 1.0 ו-TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745017"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>אין אפשרות לשלוח/לקבל דואר אלקטרוני אל/מ-Office 365 בשל היכולת של TLS 1.0 ו-TLS 1.1

כפי שאושר על-ידי מרכז ההודעות של post MC229914, TLS 1.0 ו-TLS 1.1 תבטלות התחיל לאכוף נקודות קצה של זרימת דואר מקוונת של Exchange Online. בקרוב, Office 365 לא יקבל עוד חיבורי הדואר האלקטרוני של TLS 1.0 ו-TLS 1.1 ממקורות חיצוניים. בנוסף, Exchange Online לעולם לא ישתמש ב-TLS 1.0 או ב-1.1 כדי לשלוח דואר אלקטרוני יוצא. אם אתה עומד בפני בעיות עקב היכולת של TLS 1.0 או 1.1, ייתכן שתיתקל באחת מהשגיאות הבאות-

- השולח מקבל החזרה משלוח באמצעות NDR-' 421 החיבור של 4.4.2 צנח עקב SocketError '
- שגיאה במציג התורים של שרת מקומי ששולח דואר אלקטרוני לשוטר 365-' 421 4.4.2 ' התנתק עקב SocketError '
- שגיאה [ביומן](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) שליחת פרוטוקול מחבר בשרת שולח דואר אלקטרוני אל Office 365-משאים ומתנים של TLS נכשלו עם שגיאה SocketError
- שגיאה ביומן השליחה או הקבלה של פרוטוקול מחבר-' 451 5.7.3 חייב להנפיק את הפקודה STARTTLS תחילה '

אם אתה נתקל בשגיאות שלעיל, ודא שהשרת ששולח או מקבל דואר אלקטרוני מכיל את האפשרות TLS 1.2 מופעל על-ידי בדיקת מפתחות הרישום הבאים-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ לקוח] **"DisabledByDefault" = dword: 00000000 "Enabled" = dword: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = dword: 00000000 "זמין" = dword: 00000001**

אם תבצע שינוי כלשהו במפתחות הרישום לעיל כדי להפוך את TLS 1.2 לזמין, הפעל מחדש את השרת כדי שהשינויים ייכנסו לתוקף. כמו כן, ודא שהתקנת את העדכונים האחרונים של Windows ו-Exchange.

לקבלת מידע נוסף, ראה:

- [הדרכה של Exchange Server TLS, חלק 1: התכונן לקבלת TLS 1.2-קהילת Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [חלק הדרכה של Exchange Server TLS 2: הפעלת TLS 1.2 וזיהוי לקוחות שאינם משתמשים בה-קהילת Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [הכרת תרחישי דואר אלקטרוני אם לא ניתן להסכים על גירסאות TLS באמצעות Exchange Online-קהילת Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
