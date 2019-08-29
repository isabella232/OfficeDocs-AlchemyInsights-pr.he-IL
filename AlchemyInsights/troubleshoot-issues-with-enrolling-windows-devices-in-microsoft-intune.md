---
title: פתרון בעיות ברישום התקני Windows ב-Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665833"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>פתרון בעיות ברישום התקני Windows ב-Microsoft Intune

סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה שלך כעת.
  
מספר הודעות שגיאה נפוצות ושלבי פענוח:
  
 **לא ניתן להתקין את התוכנה, 0x80cf4017:** פג תוקפו של אישור החשבון שלך. הורד מחדש את חבילת התוכנות PC Client במסוף Intune Admin. עיין בתיעוד זה לקבלת מידע נוסף.
  
 **קוד שגיאה 0x801c0003:** השגיאה יכולה להופיע בתרחישים הבאים:
  
-  למשתמש יש התקנים נוספים שנרשמו ממגבלת ההתקן. סקור מסמכים אלה [](https://docs.microsoft.com/intune/devices-wipe) כדי להסיר התקן או [לשנות את מגבלת ההתקן](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "משתמשים יכולים לצרף התקנים לתכלת AD" מוגדר "none". הגדר אותה לכל או בחר משתמשים. עיין [בתיעוד זה](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) לקבלת מידע נוסף.

-  ההתקן כבר נרשם על-ידי משתמש אחר. אם זה המקרה, להסיר את המכשיר מהמסוף Intune תכלת או לבטל ידנית את הרישום של המכשיר לפני שתנסה שוב.

-  ההתקן הוא Windows 10 Home. רק Windows 10 Pro, השכלה וארגון SKUs יכול להצטרף כחול Active ספריה.

משאבים נוספים שיסייעו בפתרון הבעיה:
  
-  השתמש [בפורטל לפתרון בעיות Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) כדי לאבחן ולפתור כשלים נפוצים בהרשמה. לפרטים נוספים, עיין [במסמך זה](https://docs.microsoft.com/intune/help-desk-operators) .

-  סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה והחלטות לכל: [מדריך לפתרון בעיות](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ולפתרון בעיות [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[למד כיצד לרשום התקני Windows ב-Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
