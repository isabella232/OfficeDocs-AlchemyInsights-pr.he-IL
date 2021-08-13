---
title: פתרון בעיות ברישום מכשירי Android Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008079"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>פתרון בעיות ברישום מכשירי Android Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.
  
כמה בעיות נפוצות ושלבי פתרון:
  
 **שגיאת התקן לא מוצפנת Company Portal:** גירסאות חדשות יותר של Android, במיוחד החל מ- v7.0, דורשות קוד סיסמה לאתחול כדי לוודא שהמכשיר שלך מוצפן באופן מלא. פתרונות נפוצים הם לאפשר הצמדת אתחול או להצפין את המכשיר באופן מלא. סקור [מסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.
  
 ההתקנים לא מצליחים לבצע צ'ק-אין עם שירות Intune או להציג אותם **כ- "Unhealthy" במסוף הניהול של Intune:** ייתכן שמכשירים מסוימים של Samsung 4.4 ו- 5.5 לא יבדקו את השירות. קיימים 3 פתרונות אפשריים לבעיה זו:
  
1. פתח באופן ידני את Intune Company Portal, אשר יוזם סינכרון מכשיר באופן אוטומטי.

2. עדכן את המכשיר ל- Android 6.0 ואילך.

3. הפוך את Samsung Smart Manager ללא זמין מניהול Intune Company Portal. סקור [מסמך זה](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים על בעיות ופתרונות אלה.

 **סוג רשיון משתמש לא** חוקי או שגיאה בשם משתמש שאינו **מזוהה:** יש להקצות למשתמש רשיון Intune או EMS. סקור מסמכים אלה כדי להקצות רשיון באמצעות: Office Admin Center או פורטל Azure.
  
משאבים נוספים שיעזור לך לפתור את הבעיה:
  
1. השתמש [בפורטל פתרון הבעיות של Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלי הרשמה נפוצים. סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.

2. סקור [מסמך זה](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות שמונעות הרשמה ופתרונות לכל אחת מהשגיאות.

3. [למד כיצד לרשום מכשירי Android ב- Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
