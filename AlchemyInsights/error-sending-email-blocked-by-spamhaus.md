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
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912349"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>שגיאה בשליחת דואר אלקטרוני: לקוח למארח חסומה באמצעות Spamhaus

כתובת ה-IP שממנו נשלחה ההודעה נמצא ברשימת החסימות בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). סיבות חוסמת Spamhaus לכלול חשבונות פרוץ, שנפרצו מחשבי שיתוף כתובת IP ציבורית ומדיניות ספק שירותי אינטרנט (ISP). תיקונים אפשריים הם:
  
- עבור הודעות נכנסות חסומים שבו אתה שולט שרת דואר אלקטרוני המקור של Office 365, עליך לקבוע את הסיבה ולהסיר את הבלוק מאתר האינטרנט Spamhaus.
    
- עבור הודעות נכנסות חסומים Office 365 שבו כתובת ה-IP של המקור שייך לאדם אחר, הבעלים כתובת צריך להסיר את הבלוק מאתר האינטרנט Spamhaus. אם כתובת IP היא על רשימת החסימות מדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית שונים או להסיר את הכתובת ה-PBL.
    
- עבור הודעות יוצאות חסומים מתוך קבוצת המחשבים שלך ב- Office 365, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות דרך שירות צד שלישי. באפשרותך להשתמש בכלי בדיקת WHOIS כדי למצוא את הבעלים של כתובת IP חסומות.
    

