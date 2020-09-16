---
title: פתרון בעיות של אירועים מהדואר האלקטרוני
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658735"
---
# <a name="troubleshooting-events-from-email"></a>פתרון בעיות של אירועים מהדואר האלקטרוני

1. אימות שהתכונה זמינה עבור תיבת הדואר: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. לאחר מכן הסתכל על ' אירועים מדואר אלקטרוני ' **מייצא את הייצוא-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. ביומני ' אירועים מדואר אלקטרוני ', אתר את InternetMessageId שמתאים לפריט בתיבת הדואר.  

4. TrustScore קובע אם הפריט נוסף או לא. אירועים יתווספו רק אם TrustScore = "מהימן".

TrustScore נקבע על-ידי מאפייני SPF, Dkim או Dmarc, הנמצאים בכותרת ההודעה.

כדי להציג מאפיינים אלה:

**Outlook בשולחן העבודה**

- פתיחת הפריט
- מאפייני קובץ->-כותרות אינטרנט של >

או

**MFCMapi**

- ניווט לפריט בתיבת הדואר הנכנס
- חפש PR_TRANSPORT_MESSAGE_HEADERS_W

מאפיינים אלה נקבעים ומוקלטים במהלך ההעברה והניתוב. לקבלת פתרון בעיות נוסף, ייתכן שתצטרך להמשיך בטיפול בתמיכה בנושאי תעבורה לגבי הכשלים ב-SPF, DKIM ו-. or DMARC.