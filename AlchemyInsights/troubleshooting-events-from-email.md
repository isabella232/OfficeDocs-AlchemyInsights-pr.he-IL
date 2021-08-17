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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105353"
---
# <a name="troubleshooting-events-from-email"></a>פתרון בעיות של אירועים מתוך דואר אלקטרוני

1. ודא שהתכונה זמינה עבור תיבת הדואר: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. לאחר מכן, הבט ביומני 'אירועים בדואר אלקטרוני' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. ביומני הרישום של 'אירועים בדואר אלקטרוני', חפש את InternetMessageId התואם לפריט בתיבת הדואר.  

4. TrustScore קובע אם הפריט נוסף או לא. אירועים יתווספו רק אם TrustScore = "Trusted".

TrustScore נקבע על-ידי מאפייני SPF, Dkim או Dmarc, הנמצאים בכותרת ההודעה.

כדי להציג מאפיינים אלה:

**שולחן Outlook**

- פתיחת הפריט
- קובץ -> מאפיינים -> כותרות אינטרנט

או

**MFCMapi**

- ניווט אל הפריט בתיבת הדואר הנכנס
- חפש את PR_TRANSPORT_MESSAGE_HEADERS_W

מאפיינים אלה נקבעים ונרשמו במהלך תעבורה וניתוב. לקבלת פתרון בעיות נוסף, ייתכן שיהיה עליך להמשך טיפול בתמיכת תעבורה לגבי הכשלים ב- SPF , DKIM ו- .או DMARC.