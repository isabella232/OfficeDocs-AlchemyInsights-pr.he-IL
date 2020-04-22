---
title: שגיאה בשליחת דואר אלקטרוני שנחסם על-ידי ספאם
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714259"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>שגיאה בשליחת דואר אלקטרוני: מארח לקוח נחסם באמצעות ספאם

כתובת ה-IP ששלחה את ההודעה נמצאת ברשימת בלוקים השייכת ל- [ספאם haus](https://go.microsoft.com/fwlink/p/?linkid=123245). הסיבות לחסימה של הדואר הזבל כוללות חשבונות פרוצים, מחשבים פרוצים המשתפים כתובת IP ציבורית ומדיניות של ספק שירותי אינטרנט (ISP). תיקונים אפשריים הם:
  
- עבור הודעות נכנסות חסומות שבהן אתה שולט בשרת הדואר האלקטרוני המהווה מקור, עליך לקבוע את הסיבה ולהסיר את הבלוק מאתר האינטרנט של ספאם.

- עבור הודעות נכנסות שנחסמו כאשר כתובת ה-IP המהווה מקור שייכת למישהו אחר, בעלי הכתובת צריך להסיר את הבלוק מאתר האינטרנט של הדואר. אם כתובת ה-IP נמצאת ברשימת בלוק המדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית שונה או להסיר את הכתובת מ-PBL.

- עבור הודעות יוצאות שנחסמו מהתחום שלך המחובר ל-Microsoft, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות באמצעות שירות צד שלישי. באפשרותך להשתמש בכלי בדיקת מWHOIS כדי למצוא את הבעלים החסומים של כתובת IP.
