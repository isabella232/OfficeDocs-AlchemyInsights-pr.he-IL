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
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387850"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>שגיאה בשליחת דואר אלקטרוני: לקוח למארח חסומה באמצעות Spamhaus

כתובת ה-IP שממנו נשלחה ההודעה נמצא ברשימת החסימות בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). סיבות חוסמת Spamhaus לכלול חשבונות פרוץ, שנפרצו מחשבי שיתוף כתובת IP ציבורית ומדיניות ספק שירותי אינטרנט (ISP). תיקונים אפשריים הם:
  
- עבור הודעות נכנסות חסומים שבו אתה שולט שרת דואר אלקטרוני המקור של Office 365, עליך לקבוע את הסיבה ולהסיר את הבלוק מאתר האינטרנט Spamhaus.

- עבור הודעות נכנסות חסומים Office 365 שבו כתובת ה-IP של המקור שייך לאדם אחר, הבעלים כתובת צריך להסיר את הבלוק מאתר האינטרנט Spamhaus. אם כתובת IP היא על רשימת החסימות מדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית שונים או להסיר את הכתובת ה-PBL.

- עבור הודעות יוצאות חסומים מתוך קבוצת המחשבים שלך ב- Office 365, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות דרך שירות צד שלישי. באפשרותך להשתמש בכלי בדיקת WHOIS כדי למצוא את הבעלים של כתובת IP חסומות.
