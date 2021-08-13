---
title: פתרון בעיות ברישום Windows מכשירים Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981042"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>פתרון בעיות ברישום Windows מכשירים Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.
  
כמה הודעות שגיאה נפוצות ושלבי פתרון:
  
 **לא ניתן להתקין את התוכנה, 0x80cf4017:** פג תוקפו של אישור החשבון שלך. הורד מחדש את חבילת התוכנה של לקוח PC במסוף הניהול של Intune. עיין בתיעוד זה לקבלת מידע נוסף.
  
 **קוד שגיאה 0x801c0003:** השגיאה עשויה להתרחש בתרחישים הבאים:
  
-  למשתמש יש יותר מכשירים שנרשמו ממגבלת המכשיר. סקור מסמכים אלה כדי להסיר [מכשיר או לשנות](https://docs.microsoft.com/intune/devices-wipe) את [מגבלת המכשיר.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "משתמשים עשויים להצטרף למכשירים ל- Azure AD" מוגדר ל- "none". הגדר אותו לכל המשתמשים או בחר אותם. עיין [בתיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.

-  המכשיר כבר רשום על-ידי משתמש אחר. במקרה זה, הסר את המכשיר ממסוף Azure Intune או בטל את ההסתה של המכשיר באופן ידני לפני ניסיון שוב.

-  המכשיר הוא Windows 10 Home. רק Windows 10 Pro, מדריכים ו- SKUs ארגוניים יכולים להצטרף ל- Azure Active Directory.

משאבים נוספים שיעזור לך לפתור את הבעיה:
  
-  השתמש [בפורטל פתרון הבעיות של Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלי הרשמה נפוצים. סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.

-  סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות שמונעות הרשמה ופתרונות לכל אחד מהם: [מדריך פתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ומסמך לפתרון בעיות.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[למד כיצד לרשום Windows במכשירים Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
