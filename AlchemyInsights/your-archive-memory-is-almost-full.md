---
title: תיבת הדואר של הארכיון שלך כמעט מלאה
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046753"
---
# <a name="your-archive-mailbox-is-almost-full"></a>תיבת הדואר של הארכיון שלך כמעט מלאה

אם המשתמש מקבל את האזהרה; **תיבת הדואר של הארכיון כמעט מלאה**, או שתצטרך להגדיל את תיבת הדואר של הארכיון, להלן כמה עצות:

1. אם למשתמש מוקצה תוכנית Exchange Online 1, שדרג **לרשיון Exchange Online 2** כדי להגדיל את הגודל מ- 50 GB ל- 100 ג'יגה-בתים.
1. אם למשתמש כבר מוקצית אחת מהפעולות **הבאות: Exchange Online תוכנית 2** או תוכנית Exchange Online 1 עם הרחבה של אחסון בארכיון של Exchange Online, השתמש בשלבים הבאים כדי להפוך אחסון אוטומטי בארכיון לזמין:
 
    1. [התחברות כדי Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. הפעל את הפקודה הבאה עבור המשתמש:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. הפעל את הפקודה הבאה כדי לאשר שהפקודה זמינה עבור המשתמש:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

לקבלת מידע נוסף, ראה:

- [הפיכת אחסון בארכיון ללא הגבלה לזמין - עזרה למנהלי מערכת - Microsoft 365 תאימות | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online - תיאורי שירות | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [שדרוג לתוכנית עסקית | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

