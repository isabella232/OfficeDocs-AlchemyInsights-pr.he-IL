---
title: פתרון בעיות ברישום מכשירי Windows ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658879"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>פתרון בעיות ברישום מכשירי Windows ב-Microsoft intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.
  
מספר הודעות שגיאה נפוצות ושלבי פתרון:
  
 **אין אפשרות להתקין את התוכנה, 0x80cf4017:** פג תוקפו של אישור החשבון שלך. הורד מחדש את חבילת תוכנת לקוח של PC במסוף הניהול של המנגינה. עיין בתיעוד זה לקבלת מידע נוסף.
  
 **קוד שגיאה 0x801c0003:** השגיאה עשויה להתרחש בתרחישים הבאים:
  
-  המשתמש מכיל מכשירים נוספים שנרשמו ממגבלת ההתקן. סקור מסמכים אלה כדי [להסיר מכשיר](https://docs.microsoft.com/intune/devices-wipe) או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "משתמשים עשויים להצטרף למכשירים לתכלת לספירה" מוגדר ל-"none". הגדר הכל או בחר משתמשים. עיין [בתיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.

-  המכשיר כבר נרשם על-ידי משתמש אחר. אם זהו המצב, הסר את ההתקן מהמסוף של ' שינוי תכלת ' או בטל את הרישום של המכשיר באופן ידני לפני שתנסה שוב.

-  המכשיר הוא Windows 10 Home. רק מחשבי Sku של Windows 10 Pro, השכלה וארגונים יכולים להצטרף לתכלת Active Directory.

משאבים נוספים שיעזרו לך לפתור את הבעיה:
  
-  השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים. סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.

-  סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ולפתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[למד כיצד לרשום מכשירי Windows ב-Microsoft intune](https://docs.microsoft.com/intune/windows-enroll).
