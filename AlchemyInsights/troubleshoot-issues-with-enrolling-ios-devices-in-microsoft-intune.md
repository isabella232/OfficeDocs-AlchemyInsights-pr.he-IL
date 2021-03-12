---
title: פתרון בעיות ברישום מכשירי iOS ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708963"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>פתרון בעיות ברישום מכשירי iOS ב-Microsoft intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת. 
  
מספר הודעות שגיאה נפוצות ושלבי פתרון:
  
- **הגעת לאות המכשירים** המשתמש מכיל מכשירים נוספים שנרשמו ממגבלת ההתקן. סקור מסמכים אלה כדי [להסיר מכשיר](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **שירות זה אינו נתמך. ללא מדיניות הרשמה:** שירות ההודעות של Apple פוש (APNS) צריך להיות מוגדר או מתחדש. סקור [מסמך זה](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) לקבלת הוראות לביצוע פעולה זו. 
    
- **סוג רשיון משתמש לא חוקי או שם משתמש אינו מזוהה:** יש להקצות למשתמש רשיון כוונון או EMS. סקור מסמכים אלה כדי להקצות רשיון דרך: [מרכז הניהול של Office](https://docs.microsoft.com/intune/licenses-assign) או [פורטל התכלת](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
משאבים נוספים שיעזרו לך לפתור את הבעיה:
  
1. השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים. סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים. 
    
2. סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ולפתרון בעיות](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [למד כיצד לרשום מכשירי iOS ב-Microsoft intune](https://docs.microsoft.com/intune/ios-enroll).
    

