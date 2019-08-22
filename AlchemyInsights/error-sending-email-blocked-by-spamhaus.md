---
title: שגיאה בשליחת דואר אלקטרוני נחסם על-ידי SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527134"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>שגיאה בשליחת דואר אלקטרוני: לקוח למארח חסומה באמצעות Spamhaus

כתובת ה-IP שממנו נשלחה ההודעה נמצא ברשימת החסימות בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). סיבות חוסמת Spamhaus לכלול חשבונות פרוץ, שנפרצו מחשבי שיתוף כתובת IP ציבורית ומדיניות ספק שירותי אינטרנט (ISP). תיקונים אפשריים הם:
  
- עבור הודעות נכנסות חסומים שבו אתה שולט שרת דואר אלקטרוני המקור של Office 365, עליך לקבוע את הסיבה ולהסיר את הבלוק מאתר האינטרנט Spamhaus.

- עבור הודעות נכנסות חסומים Office 365 שבו כתובת ה-IP של המקור שייך לאדם אחר, הבעלים כתובת צריך להסיר את הבלוק מאתר האינטרנט Spamhaus. אם כתובת IP היא על רשימת החסימות מדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית שונים או להסיר את הכתובת ה-PBL.

- עבור הודעות יוצאות חסומים מתוך קבוצת המחשבים שלך ב- Office 365, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות דרך שירות צד שלישי. באפשרותך להשתמש בכלי בדיקת WHOIS כדי למצוא את הבעלים של כתובת IP חסומות.
