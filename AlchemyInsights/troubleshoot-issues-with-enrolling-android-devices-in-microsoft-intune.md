---
title: פתרון בעיות עם רושם התקנים Android ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420593"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>פתרון בעיות עם רושם התקנים Android ב- Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.
  
מספר בעיות נפוצות ושלבי פתרון:
  
 **בהתקן אינם מוצפנים שגיאה בפורטל החברה:** גירסאות חדשות יותר של Android, v7.0, במיוחד החל לדרוש passcode האתחול כדי לוודא כי ההתקן שלך מוצפן באופן מלא. פתרונות נפוצים הם כדי להפוך pin האתחול או להצפין את ההתקן באופן מלא. סקירת [מסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף. 
  
 **התקנים להיכשל לבדוק באמצעות השירות Intune או להציג כ- "Unhealthy" במסוף הניהול Intune:** 4.4 Samsung מסוימים והתקני 5.5 ייתכן תסמן לתוך השירות. ישנם 3 פתרונות אפשריים לבעיה זו: 
  
1. פתח app פורטל החברה Intune, אשר באופן אוטומטי יאתחל סינכרון ההתקן באופן ידני.
    
2. עדכן את ההתקן כדי Android 6.0 ומעלה.
    
3. ביטול מנהל חכם Samsung מניהול הפורטל החברה Intune. סקירת [מסמך זה](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים על בעיות ופתרונות אלה. 
    
 **סוג חוקי של רשיון משתמש** או **משתמש שם לא מזוהה שגיאה:** שעל המשתמש שיש להקצות רשיון Intune או EMS. סקירת מסמכים אלה כדי להקצות רשיון דרך: פורטל מרכז הניהוליים של Office או תכלת הרקיע. 
  
משאבים נוספים כדי לסייע לפתור את הבעיה:
  
1. להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות. סקירת [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים. 
    
2. סקירת [מסמך זה](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל. 
    
3. [למד כיצד לרשום התקנים Android ב- Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

