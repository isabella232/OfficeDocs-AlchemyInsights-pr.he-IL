---
title: פתרון בעיות בפריסת אישור של אימות לקוח
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555309"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>פתרון בעיות בפריסת אישור של אימות לקוח

פרופילי אישורי לקוח Intune NDES/SCEP ו-PKCS/PFX משמשים בדרך כלל בשילוב עם סוגי פרופילים אחרים כגון Wifi, VPN ודוא ל כדי לאפשר למשתמשים לבצע אימות למשאבי החברה. כאשר סוגי פרופילים אלה מקושרים לפרופיל של אישור לקוח תלויים בפריסה המוצלחת של פרופיל זה.

הגדרת תשתית ראשונית ותצורה משויכת של הפרופיל של אישור הלקוח דורשות לעתים קרובות פתרון בעיות. לקבלת מדריך שלב אחר שלב לכיוונון מוצלח של מחבר NDES ולפתרון בעיות הדרכה לבידוד בעיות בפריסת האישורים, ראה: 

- [קביעת תצורה של תשתית לתמיכה ב-SCEP עם Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [סקירה כללית של פתרון בעיות בפרופילי אישורים של SCEP עם Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

השתמש בסקריפטים שאליהם מפנה powershell כדי לסייע באימות התצורה. לקבלת מידע נוסף, ראה [Intune סקריפטים לאימות מחבר אישור](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**סוגיות נפוצות אחרות**

**כאשר אני מנסה להתקין את מחבר האישור Intune בשרת המחבר NDES, אני מקבל את ההודעה "אין אפשרות לאמת את הסיסמה בבקשת האישור. . ייתכן שכבר השתמשו בו השג סיסמה חדשה לשליחה באמצעות בקשה זו. "**  

הודעה זו פירושה שעליך להפעיל את התקנת מחבר האישורים כמנהל.

בסביבות מסוימות, השרתים שבהם האישור Intune פועל חייבים להשתמש בשרת proxy כדי להתחבר ל-Intune ולכן מחבר האישורים חייב להשתמש ב-proxy. בנסיבות מסוימות, מחבר NDES מתעלם מהגדרות ה-proxy שהוגדרו וייתכן שיהיה צורך לקבוע את תצורת הגדרות ה-proxy בעת הפעלה בהקשר האבטחה של LocalSystem. 
 
הפתרון הוא להפעיל את Internet Explorer כמערכת ולהגדיר proxy ב-IE. לאחר הפעלה מחדש של שירות מחבר Intune, מחבר NDES מתחבר לIntune.

**התקני משתמש אינם מקבלים עוד אישורי SCEP מ-NDES.**

ייתכן שאישור אימות הלקוח הונפק לשרת NDES ושצוין במהלך התקנת מחבר NDES, פג תוקפו או שחסר. כדי לפתור: 
 
1. הסר את ההתקנה של מחבר NDES.  
2. השתמש בפרטים אלה כדי לבקש אימות חדש של לקוח או אישור אימות שרת: 
 
    - שם הנושא: CN = fqdn חיצוני  
    - שם חלופי של נושא (שניהם נדרשים): DNS = fqdn חיצוני, DNS = fqdn פנימי 
 
3. התקן מחדש את מחבר NDES באישור החדש.