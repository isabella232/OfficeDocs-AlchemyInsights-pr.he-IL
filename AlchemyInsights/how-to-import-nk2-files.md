---
title: כיצד לבצע ייבוא-nk2-קבצים
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
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780060"
---
# <a name="how-to-import-nk2-files"></a>כיצד לייבא קבצי. nk2 

כאשר אתה מפעיל את Microsoft Outlook 2013, Outlook 2016, Outlook 2019 או Outlook עבור Microsoft 365 בפעם הראשונה, מטמון הכינוי שלך (מאוחסן בקובץ *profilename*. nk2) מיובא להודעה מוסתרת במאגר ההודעות המשמש כברירת מחדל.

כדי לייבא קבצי. nk2 ל-Outlook 2013, Outlook 2016, Outlook 2019 או Outlook עבור Microsoft 365, ודא שהקובץ. nk2 נמצא בתיקיה הבאה:%appdata%\Microsoft\Outlook

**הערה**: קובץ ה-. nk2 חייב להיות בעל שם זהה לזה של outlook 2013 או outlook 2016 הנוכחי. כברירת מחדל, שם הפרופיל הוא "Outlook". כדי לבדוק את שם הפרופיל, בצע את הפעולות הבאות: 
1. לחץ על **התחל** ולאחר מכן לחץ על **לוח הבקרה**.
2. לחץ פעמיים על **דואר**.
3. בתיבת הדו הגדרת דואר, בחר באפשרות **הציגו פרופילים**.
4. בחר **התחל**  >  **הפעל**.
5. בתיבה **פתח** את, הקלד * outlook.exe /importnk2*ולאחר מכן בחר **אישור**. 

לאחר ייבוא קובץ ה-. nk2, תוכן הקובץ ממוזג למטמון הכינוי הקיים המאוחסן בתיבת הדואר שלך.

**הערה**: הקובץ. nk2 משתנה עם סיומת שם הקובץ. old בפעם הבאה שתפעיל את outlook 2013, outlook 2016, outlook 2019 או Outlook עבור Microsoft 365. אם ברצונך לייבא מחדש את הקובץ. nk2, הסר תחילה את סיומת שם הקובץ הישנה.

לקבלת מידע נוסף, ראה [ייבוא או העתקה של רשימת ההשלמה האוטומטית למחשב אחר](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).