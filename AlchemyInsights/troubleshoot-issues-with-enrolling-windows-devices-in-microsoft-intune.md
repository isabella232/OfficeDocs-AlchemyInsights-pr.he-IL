---
title: פתרון בעיות עם רושם התקני Windows ב- Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934777"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>פתרון בעיות עם רושם התקני Windows ב- Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת. 
  
כמה הודעות שגיאה נפוצות ושלבי פתרון:
  
 **אין אפשרות להתקין את התוכנה, 0x80cf4017:** פג תוקפו של האישור לחשבון שלך. להוריד מחדש את חבילת התוכנה הלקוח מחשב אישי במסוף הניהול Intune. סקירת תיעוד זה לקבלת מידע נוסף. 
  
 **קוד השגיאה 0x801c0003:** השגיאה עלולה להתרחש בתרחישים הבאים: 
  
1. למשתמש יש יותר התקנים שנרשמו ממגבלת המכשיר. סקירת מסמכים אלה כדי [להסיר התקן](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת התקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "משתמשים עשויים להצטרף התקנים כדי AD תכלת הרקיע" מוגדרת ל- "none". להגדיר אותו לכל או בחר משתמשים. סקירת [תיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף. 
    
3. ההתקן כבר נרשם על-ידי משתמש אחר. אם זהו המקרה, הסר את ההתקן מהמסוף תכלת הרקיע Intune או unenroll את ההתקן באופן ידני לפני שתנסה שוב.
    
4. ההתקן הוא 10 Windows Home. רק Pro 10 של Windows, חינוך ואת פריטי ה-Sku של הארגון יכולים להצטרף תכלת הרקיע Active Directory.
    
משאבים נוספים כדי לסייע לפתור את הבעיה:
  
1. להשתמש [בפורטל פתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים הרשמה נפוצות. סקירת [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים. 
    
2. סקירת מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ופתרונות לכל: [מדריך פתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ו- [doc ופתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[למד כיצד לרשום התקני Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

