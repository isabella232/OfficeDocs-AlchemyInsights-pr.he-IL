---
title: שגיאה בשליחת דואר אלקטרוני שנחסם על-ידי SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813725"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>שגיאה בשליחת דואר אלקטרוני: מארח הלקוח נחסם באמצעות Spamhaus

כתובת ה- IP ששלחה את ההודעה נמצאת ברשימת חסימות בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). הסיבות לחסומים על-ידי Spamhaus כוללות חשבונות שנפגמו, מחשבים שנפגמו בסכנה החולקים כתובת IP ציבורית ומדיניות ספק שירותי אינטרנט (ISP). תיקונים אפשריים הם:
  
- עבור הודעות נכנסות חסומות במקום שבו אתה שולט בשרת הדואר האלקטרוני המשמש כמקור, עליך לקבוע את הגורם ולהסיר את הבלוק מהאתר של Spamhaus.

- עבור הודעות נכנסות חסומות שייכות לכתובת ה- IP המשמשת כמקור למישהו אחר, בעל הכתובת צריך להסיר את הבלוק מהאתר של Spamhaus. אם כתובת ה- IP נמצאת ברשימת בלוקי המדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית אחרת או להסיר את הכתובת מה- PBL.

- עבור הודעות יוצאות חסומות מהתחום המחובר ל- Microsoft, באפשרותך לקבל שגיאה זו אם ההודעות מנותב דרך שירות של ספקים שלישיים. באפשרותך להשתמש בכלי בדיקת מידע של WHOIS כדי למצוא את הבעלים של כתובת ה- IP החסומים.
