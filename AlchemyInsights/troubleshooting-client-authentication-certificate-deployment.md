---
title: פתרון בעיות בפריסת אישור אימות לקוח
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020805"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>פתרון בעיות בפריסת אישור אימות לקוח

פרופילי אישורי לקוח Intune NDES/SCEP ו- PKCS/PFX משמשים בדרך כלל בשילוב עם סוגי פרופילים אחרים, כגון Wifi, VPN ודעת דואר אלקטרוני כדי לאפשר למשתמשים לבצע אימות למשאבים ארגוניים. כאשר סוגי פרופילים אלה מקושרים לפרופיל אישור לקוח תלויים בפריסה המוצלחת של פרופיל זה.

הגדרת תשתית ראשונית ותצורה משויכת של פרופיל אישור הלקוח דורשות לעתים קרובות פתרון בעיות. לקבלת מדריך שלב אחר שלב להגדרה מוצלחת של מחבר NDES והדרכה לפתרון בעיות לבודד בעיות בפריסת אישורים, ראה: 

- [קביעת תצורה של תשתית לתמיכה ב- SCEP עם Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [מבט כולל על פתרון בעיות בפרופילי אישורי SCEP עם Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

השתמש בקבצי ה- Script של Powershell שאליהם בוצעה הפניה כדי לסייע באימות התצורה שלך. לקבלת מידע נוסף, ראה [קבצי Script של אימות מחבר אישור Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**בעיות נפוצות אחרות**

**כאשר אני מנסה להתקין את מחבר האישור Intune בשרת המחבר של NDES, אני מקבל את ההודעה, "לא ניתן לאמת את הסיסמה בבקשה לאישור. ייתכן שכבר נעשה בו שימוש. השג סיסמה חדשה לשליחה באמצעות בקשה זו."**  

הודעה זו פירושה שתצטרך להפעיל את התקנת מחבר האישור כמנהל מערכת.

בסביבות מסוימות, השרתים היכן שאישור Intune פועל חייבים להשתמש בשרת Proxy כדי להתחבר ל- Intune, ולכן מחבר האישורים חייב להשתמש ב- Proxy. בנסיבות מסוימות, מחבר NDES מתעלם מהגדרות ה- Proxy שהוגדרו, וייתכן שיהיה צורך לקבוע את תצורת הגדרות ה- Proxy בעת הפעלתן בהקשר האבטחה של LocalSystem. 
 
הפתרון הוא להפעיל את Internet Explorer כ- SYSTEM ולהגדיר Proxy ב- IE. לאחר הפעלה מחדש של שירות המחבר Intune, מחבר NDES מתחבר ל- Intune.

**מכשירי משתמש אינם מקבלים עוד אישורי SCEP מ- NDES.**

ייתכן שאישור אימות הלקוח שהונפק לשרת NDES, וצוין במהלך התקנת מחבר NDES, פג או חסר. כדי לפתור: 
 
1. הסר את התקנת מחבר NDES.  
2. השתמש בפרטים אלה כדי לבקש אישור אימות לקוח או אימות שרת חדש: 
 
    - שם נושא: CN=external fqdn  
    - שם חלופי של נושא (שניהם נדרשים): DNS=external fqdn, DNS=internal fqdn 
 
3. התקן מחדש את מחבר NDES באמצעות האישור החדש.