---
title: פתרון בעיות ברישום מכשירי Android ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708999"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>פתרון בעיות ברישום מכשירי Android ב-Microsoft intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.
  
כמה בעיות נפוצות ושלבי פתרון:
  
 **שגיאה לא מוצפנת של התקן בפורטל החברה:** גירסאות חדשות יותר של Android, במיוחד החל מ-v 7.0, דורשות סיסמה של הפעלה כדי לוודא שההתקן שלך מוצפן במלואו. פתרונות נפוצים משמשים להפיכת מספר זיהוי אישי של הפעלה לזמין או להצפנה מלאה של המכשיר. סקור [מסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.
  
 **המכשירים אינם מצליחים להיכנס באמצעות שירות ה-intune או הצג כ-"לא בריא" במסוף הניהול של intune:** ייתכן שמכשירים מסוימים של Samsung 4.4 ו-5.5 לא ייכנסו לשירות. קיימים 3 פתרונות אפשריים לבעיה זו:
  
1. פתח באופן ידני את יישום הפורטל של כוונון החברה, שייזום באופן אוטומטי סינכרון מכשיר.

2. עדכן את המכשיר ל-Android 6.0 ואילך.

3. הפוך את סמסונג Smart Manager ללא זמין מניהול הפורטל של החברה. סקור [מסמך זה](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים על בעיות ופתרונות אלה.

 **סוג רשיון של משתמש לא חוקי** או **שם משתמש לא זוהה שגיאה:** המשתמש צריך להקצות לו רשיון של כוונון או EMS. סקור מסמכים אלה כדי להקצות רשיון דרך: מרכז הניהול של Office או פורטל התכלת.
  
משאבים נוספים שיעזרו לך לפתור את הבעיה:
  
1. השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים. סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.

2. סקור [מסמך זה](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן.

3. [למד כיצד לרשום מכשירים של Android ב-Microsoft intune](https://docs.microsoft.com/intune/android-enroll).
