---
title: תיבת הדואר שלך בארכיון כמעט מלאה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974404"
---
# <a name="your-archive-mailbox-is-almost-full"></a>תיבת הדואר שלך בארכיון כמעט מלאה

אם המשתמש מקבל את האזהרה; **תיבת הדואר שלך בארכיון כמעט מלאה**, או אם עליך להגדיל את תיבת הדואר של הארכיון שלהם, הנה כמה עצות:

1. אם למשתמש הוקצה תוכנית Exchange Online 1, שדרג את הרשיון **לתוכנית Exchange online 2** כדי להגדיל את הגודל מ-50 GB ל-100GB.
1. אם המשתמש כבר מוקצה לאחת מהאפשרויות הבאות: **Exchange Online plan 2** או תוכנית exchange online 1 עם התוספת לאחסון בארכיון של exchange online, השתמש בשלבים שלהלן כדי להפוך אחסון מתרחב אוטומטי לזמין:.
 
    1. [התחבר אל Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. הפעלת הunifiedgroup הבאים עבור המשתמש:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. הפעלת הunifiedgroup הבאים כדי לאשר שהוא זמין עבור המשתמש:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

לקבלת מידע נוסף, ראה:

- [ הפיכת אחסון בלתי מוגבל לזמין בארכיון-עזרה למנהלי מערכת-תאימות של Microsoft 365 | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [מגבלות Exchange Online-תיאורי שירותים | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [שדרג לתוכנית עסקית אחרת | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

