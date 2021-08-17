---
title: פתרון בעיות ברישום מכשירי iOS ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047977"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>פתרון בעיות ברישום מכשירי iOS ב- Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת. 
  
כמה הודעות שגיאה נפוצות ושלבי פתרון:
  
- **הגעת למכסה המכשיר** למשתמש יש יותר מכשירים שנרשמו ממגבלת המכשיר. סקור מסמכים אלה כדי להסיר [מכשיר או לשנות](https://docs.microsoft.com/intune/devices-wipe) את [מגבלת המכשיר.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **שירות זה אינו נתמך. אין צורך לקבוע את התצורה** או החידוש של שירות הודעות דחיפה (APNS) של Apple. עיין [במסמך](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) זה לקבלת הוראות כיצד לעשות זאת. 
    
- **סוג רשיון משתמש לא חוקי או שם משתמש אינו מזוהה:** יש להקצות למשתמש רשיון Intune או EMS. סקור מסמכים אלה כדי להקצות רשיון באמצעות: [Office Admin Center או](https://docs.microsoft.com/intune/licenses-assign) פורטל [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
משאבים נוספים שיעזור לך לפתור את הבעיה:
  
1. השתמש [בפורטל פתרון הבעיות של Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלי הרשמה נפוצים. סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים. 
    
2. סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות שמונעות הרשמה ופתרונות לכל אחד מהם: [מדריך פתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ומסמך לפתרון בעיות.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [למד כיצד לרשום מכשירי iOS ב- Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

