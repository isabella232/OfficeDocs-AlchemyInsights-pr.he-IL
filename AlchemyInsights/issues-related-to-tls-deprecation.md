---
title: לא ניתן לשלוח/לקבל דואר אלקטרוני אל/Office 365 עקב ביטול TLS 1.0 ו- TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054907"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>לא ניתן לשלוח/לקבל דואר אלקטרוני אל/Office 365 עקב ביטול TLS 1.0 ו- TLS 1.1

כפי שאושר על-ידי מרכז ההודעות לפרסם MC229914, TLS 1.0 ו- TLS 1.1 deprecation התחיל לאלץ עבור Exchange Online נקודות קצה של זרימת דואר. בקרוב Office 365 לא תקבל עוד חיבורי דואר אלקטרוני של TLS 1.0 ו- TLS 1.1 ממקורות חיצוניים. כמו כן, Exchange Online לעולם לא ישתמש ב- TLS 1.0 או ב- 1.1 כדי לשלוח דואר אלקטרוני יוצא. אם אתה נתקל בבעיות עקב ביטול TLS 1.0 או 1.1, ייתכן שתתקל באחת מהשגיאות הבאות:

- השולח מקבל חזרה את NDR - '421 4.4.2 החיבור ששוחרר עקב SocketError'
- שגיאה במציג התורים של השרת המקומי ששולח דואר אלקטרוני לקצין 365- '421 4.4.2 החיבור הושמטו עקב SocketError'
- שגיאה ביומן 'שלח [פרוטוקול מחבר'](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) בשרת השולח דואר אלקטרוני Office 365- משא ומתן של TLS נכשל עם שגיאת SocketError
- שגיאה ביומן פרוטוקול שליחה או קבלה של מחבר - '451 5.7.3 חייב להנפיק תחילה פקודת STARTTLS'

אם אתה נתקל באחד מהשגיאות לעיל, ודא שהשרת ששולח או מקבל דואר אלקטרוני כולל TLS 1.2 זמין על-ידי בדיקת מפתחות הרישום הבאים-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

אם תבצע שינוי כלשהו במפתחות הרישום שלעיל כדי להפוך את TLS 1.2 לזמין, הפעל מחדש את השרת כדי שהשינויים ייכנסו לתוקף. כמו כן, ודא שהתקנת את עדכוני Windows והעדכונים Exchange האחרונים.

לקבלת מידע נוסף, ראה:

- [Exchange Server הדרכה של TLS, חלק 1: מתכונן ל- TLS 1.2 - קהילת Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server הדרכה של TLS חלק 2: הפעלת TLS 1.2 וזיהוי לקוחות שלא משתמשים בו - קהילת Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [הבנת תרחישי דואר אלקטרוני אם לא ניתן להסכים על גירסאות TLS עם Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
