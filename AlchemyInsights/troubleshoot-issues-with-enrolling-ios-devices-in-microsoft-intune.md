---
title: פתרון בעיות עם רושם iOS התקנים ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391008"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>פתרון בעיות עם רושם iOS התקנים ב- Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת. 
  
כמה הודעות שגיאה נפוצות ושלבי פתרון:
  
- **כיפה ההתקן הגיע** למשתמש יש יותר התקנים שנרשמו ממגבלת המכשיר. סקירת מסמכים אלה כדי [להסיר התקן](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת התקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **שירות זה אינו נתמך. אין מדיניות הרשמה:** תפוח לדחוף דיווח שירות (ולמפעיל) צריך להיות מוגדר או לחדש. סקירת [מסמך זה](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) לקבלת הוראות אודות אופן ביצוע פעולה זו. 
    
- **סוג רשיון משתמש לא חוקי או לא מזוהה שם משתמש:** המשתמש צריך להקצות רשיון Intune או EMS. סקירת מסמכים אלה כדי להקצות רשיון דרך: [מרכז הניהוליים של Office](https://docs.microsoft.com/intune/licenses-assign) או [פורטל תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
משאבים נוספים כדי לסייע לפתור את הבעיה:
  
1. להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות. סקירת [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים. 
    
2. סקירת מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל: [מדריך פתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ו- [doc ופתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [למד כיצד לרשום iOS התקנים ב- Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

