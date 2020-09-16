---
title: פתרון בעיות בפריסה של אישורי אימות לקוח
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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658987"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>פתרון בעיות בפריסה של אישורי אימות לקוח

פרופילי אישורי לקוח של NDES/SCEP ו-PKCS/PFX משמשים בדרך כלל בשילוב עם סוגי פרופילים אחרים כגון Wifi, VPN ודואר אלקטרוני כדי לאפשר למשתמשים לבצע אימות למשאבי חברה. כאשר סוגי פרופילים אלה מקושרים לפרופיל אישור לקוח, תלויים הפריסה המוצלחת של פרופיל זה.

הגדרת התשתית הראשונית והתצורה המשויכת של פרופיל אישורי לקוח דורשים לעתים קרובות פתרון בעיות. לקבלת מדריך שלב-אחר-שלב להגדרה מוצלחת של מחבר NDES והדרכה לפתרון בעיות כדי לבודד בעיות בפריסת אישורים, ראה: 

- [קביעת תצורה של תשתית לתמיכה ב-SCEP באמצעות ' כוונון '](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [מבט כולל לפתרון בעיות של פרופילי אישורים SCEP עם Microsoft intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

השתמש בקבצי ה-script של powershell שאליהם הפניה כדי לסייע באימות התצורה שלך. לקבלת מידע נוסף, ראה [שלחן סקריפטים של אימות מחבר אישור](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**בעיות נפוצות אחרות**

**כאשר אני מנסה להתקין את מחבר אישור ה-intune בשרת מחבר NDES, אני מקבל את ההודעה "אין אפשרות לאמת את הסיסמה בבקשת האישור. ייתכן שכבר נעשה בה שימוש. קבל סיסמה חדשה לשליחה באמצעות בקשה זו.**  

הודעה זו משמעותה שעליך להפעיל את התקנת מחבר האישורים כמנהל מערכת.

בסביבות מסוימות, השרתים שבהם מופעל אישור ה-intune חייב להשתמש בשרת proxy כדי להתחבר למנגינה, ולכן מחבר האישור חייב להשתמש ב-proxy. בנסיבות מסוימות, מחבר NDES מתעלם מהגדרות ה-proxy שהוגדרו, וייתכן שיהיה צורך לקבוע את התצורה של הגדרות ה-proxy בעת הפעלת ההקשר הביטחוני של LocalSystem. 
 
הפתרון הוא להפעלת Internet Explorer כמערכת ולקביעת התצורה של proxy ב-IE. לאחר הפעלה מחדש של שירות מחבר המנגינה, מחבר NDES מתחבר לכיוון המנגינה.

**התקני משתמשים אינם מקבלים עוד אישורי SCEP מ-NDES.**

ייתכן שאישור אימות הלקוח הונפק לשרת NDES, ושצוין במהלך התקנת מחבר NDES, פג תוקפו או חסר. כדי לפתור: 
 
1. הסר את התקנת מחבר NDES.  
2. השתמש בפרטים אלה כדי לבקש אישור חדש לגבי אימות לקוח או אימות שרת: 
 
    - שם הנושא: CN = fqdn החיצוני  
    - שם חלופי של נושא (שניהם נדרשים): DNS = fqdn החיצוני, DNS = fqdn הפנימי 
 
3. התקן מחדש את מחבר NDES באמצעות האישור החדש.