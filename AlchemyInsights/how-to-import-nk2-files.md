---
title: כיצד לייבא-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043207"
---
# <a name="how-to-import-nk2-files"></a>כיצד לייבא קבצי .nk2 

בעת הפעלת Microsoft Outlook 2013, Outlook 2016, Outlook 2019 או Microsoft 365 של Outlook בפעם הראשונה, מטמון הכינויים (המאוחסן בקובץ .nk2 *profilename)* מיובא להודעה מוסתרת בחנות ההודעות המוגדרת כברירת מחדל.

כדי לייבא קבצי .nk2 לתוך Outlook 2013, Outlook 2016, Outlook 2019 או Microsoft 365 של Outlook, ודא שהקובץ .nk2 נמצא בתיקיה הבאה: %appdata%\Microsoft\Outlook

**הערה:** לקובץ .nk2 חייב להיות שם זהה לזה של Outlook הנוכחי שלך או Outlook 2016 שלך. כברירת מחדל, שם הפרופיל הוא "Outlook". כדי לבדוק את שם הפרופיל, בצע את הפעולות הבאות: 
1. לחץ על **התחל** ולאחר מכן לחץ על **לוח הבקרה**.
2. לחץ פעמיים על **דואר**.
3. בתיבת הדו-שיח הגדרת דואר, בחר **הצג פרופילים**.
4. בחרו **התחל** > **הפעל**.
5. בתיבה **פתח,** הקלד *outlook.exe /importnk2* ולאחר מכן בחר **אישור**. 

לאחר ייבוא קובץ .nk2, תוכן הקובץ ממוזג למטמון הכינויים הקיים המאוחסן בתיבת הדואר שלך.

**הערה:** שם הקובץ .nk2 השתנה עם סיומת שם קובץ .old בפעם הבאה שתחיל את Outlook 2013, Outlook 2016, Outlook 2019 או Microsoft 365 של Outlook. אם ברצונך לייבא מחדש את קובץ ה- .nk2, הסר תחילה את סיומת שם הקובץ .old.

לקבלת מידע נוסף, ראה [ייבוא או העתקה של רשימת ההשלמה האוטומטית למחשב אחר.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)