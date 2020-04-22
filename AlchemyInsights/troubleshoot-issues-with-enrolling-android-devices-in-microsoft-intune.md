---
title: פתרון בעיות ברישום התקני אנדרואיד ב-Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759621"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>פתרון בעיות ברישום התקני אנדרואיד ב-Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה שלך כעת.
  
מספר שלבים נפוצים של בעיות ורזולוציות:
  
 **התקן לא שגיאה מוצפנת בפורטל החברה:** גירסאות חדשות יותר של Android, המתחילות במיוחד ב-v 7.0, דורשות קוד סיסמה של הפעלה כדי לוודא שההתקן שלך מוצפן במלואו. פתרונות נפוצים הם לאפשר לפין הפעלה או להצפין את ההתקן במלואו. עיין [במסמך זה](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) לקבלת מידע נוסף.
  
 **התקנים אינם מצליחים לבצע צ'ק-אין בשירות Intune או להציג אותם כ"בלתי בריאים" במסוף מנהל Intune:** חלק סמסונג 4.4 ו-5.5 התקנים עשויים לא לבדוק את השירות. קיימים 3 פתרונות אפשריים לבעיה זו:
  
1. פתח באופן ידני את יישום הפורטל של Intune Company, אשר תיזום באופן אוטומטי סינכרון התקן.

2. עדכן את המכשיר אנדרואיד 6.0 או יותר.

3. להשבית את סמסונג מנהל חכם מניהול פורטל החברה Intune. עיין [במסמך זה](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) לקבלת פרטים נוספים אודות בעיות והחלטות אלה.

 **סוג רשיון משתמש לא חוקי** או **שם משתמש לא זוהה שגיאה:** יש להקצות למשתמש רשיון Intune או EMS. סקור מסמכים אלה כדי להקצות רשיון באמצעות: מרכז הניהול של Office או פורטל התכלת.
  
משאבים נוספים שיסייעו בפתרון הבעיה:
  
1. השתמש [בפורטל לפתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים נפוצים בהרשמה. לפרטים נוספים, עיין [במסמך זה](https://docs.microsoft.com/intune/help-desk-operators) .

2. סקור [מסמך זה](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) לקבלת רשימה של שגיאות נפוצות המונעות כל אחת מההרשמה והרזולוציות.

3. [למד כיצד לרשום התקנים אנדרואיד ב-Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
