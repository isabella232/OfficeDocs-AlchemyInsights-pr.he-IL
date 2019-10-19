---
title: פתרון בעיות ברישום התקני iOS ב-Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506966"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>פתרון בעיות ברישום התקני iOS ב-Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה שלך כעת. 
  
מספר הודעות שגיאה נפוצות ושלבי פענוח:
  
- **הגעת למכסה ההתקן** למשתמש יש התקנים נוספים שנרשמו ממגבלת ההתקן. סקור [מסמכים אלה כדי להסיר התקן](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **שירות זה אינו נתמך. אין מדיניות הרשמה:** שירות הודעות לדחיפת Apple (APNS) צריך להיות מוגדר או מתחדש. עיין [במסמך זה](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) לקבלת הוראות כיצד לעשות זאת. 
    
- **סוג רשיון משתמש לא חוקי או שם משתמש לא זוהה:** יש להקצות למשתמש רשיון Intune או EMS. סקור מסמכים אלה כדי להקצות רשיון באמצעות: [מרכז הניהול של Office](https://docs.microsoft.com/intune/licenses-assign) או [פורטל התכלת](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
משאבים נוספים שיסייעו בפתרון הבעיה:
  
1. השתמש [בפורטל לפתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים נפוצים בהרשמה. לפרטים נוספים, עיין [במסמך זה](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה והחלטות לכל: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ולפתרון בעיות doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [למד כיצד לרשום התקני iOS ב-Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

