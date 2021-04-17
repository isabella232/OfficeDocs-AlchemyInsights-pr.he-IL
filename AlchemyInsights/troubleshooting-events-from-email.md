---
title: פתרון בעיות של אירועים מתוך דואר אלקטרוני
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834840"
---
# <a name="troubleshooting-events-from-email"></a>פתרון בעיות של אירועים מתוך דואר אלקטרוני

1. ודא שהתכונה זמינה עבור תיבת הדואר: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. לאחר מכן, הבט ביומני 'אירועים בדואר אלקטרוני' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. ביומני הרישום של 'אירועים בדואר אלקטרוני', חפש את InternetMessageId התואם לפריט בתיבת הדואר.  

4. TrustScore קובע אם הפריט נוסף או לא. אירועים יתווספו רק אם TrustScore = "Trusted".

TrustScore נקבע על-ידי מאפייני SPF, Dkim או Dmarc, הנמצאים בכותרת ההודעה.

כדי להציג מאפיינים אלה:

**Outlook לשולחן העבודה**

- פתיחת הפריט
- קובץ -> מאפיינים -> כותרות אינטרנט

או

**MFCMapi**

- ניווט אל הפריט בתיבת הדואר הנכנס
- חפש את PR_TRANSPORT_MESSAGE_HEADERS_W

מאפיינים אלה נקבעים ונרשמו במהלך תעבורה וניתוב. לקבלת פתרון בעיות נוסף, ייתכן שיהיה עליך להמשך טיפול בתמיכת תעבורה לגבי הכשלים ב- SPF , DKIM ו- .או DMARC.