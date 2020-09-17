---
title: שגיאה בעת שליחת דואר אלקטרוני נחסם על-ידי SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783804"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>שגיאה בעת שליחת דואר אלקטרוני: מארח לקוח נחסם באמצעות Spamhaus

כתובת ה-IP ששלחה את ההודעה נמצאת ברשימת חסימות הנמצאת בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). הסיבות לחסימת הSpamhaus כוללות חשבונות שנחשפו, מחשבים שנפרצו שיתוף כתובת IP ציבורית ומדיניות של ספק שירותי אינטרנט (ISP). תיקונים אפשריים הם:
  
- לקבלת הודעות נכנסות שנחסמו כאשר אתה שולט בשרת הדואר האלקטרוני המשמש כמקור, עליך לקבוע את הסיבה ולהסיר את החסימה מאתר האינטרנט של Spamhaus.

- עבור הודעות נכנסות שנחסמו כאשר כתובת ה-IP של המקור שייכת לאדם אחר, בעלי הכתובת צריך להסיר את הבלוק מאתר האינטרנט של Spamhaus. אם כתובת ה-IP נמצאת ברשימת חסימות המדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית אחרת או להסיר את הכתובת מ-PBL.

- עבור הודעות יוצאות שנחסמו מהתחום שלך המחובר ל-Microsoft, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות באמצעות שירות של צד שלישי. באפשרותך להשתמש בכלי בדיקת מידע של WHOIS כדי למצוא את הבעלים של כתובת ה-IP החסומה.
