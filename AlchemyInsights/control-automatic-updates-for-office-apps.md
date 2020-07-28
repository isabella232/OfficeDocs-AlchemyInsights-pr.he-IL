---
title: שלוט בעדכונים אוטומטיים עבור יישומי Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439332"
---
# <a name="control-automatic-updates-for-office-apps"></a>שלוט בעדכונים אוטומטיים עבור יישומי Office

כברירת מחדל, עדכונים עבור יישומי Office מורדים באופן אוטומטי ומוחלים ברקע ללא התערבות של המשתמש. עם זאת, מנהלי מערכת יכולים לשלוט באופן החלת העדכונים באמצעות הגדרות Office Update. הגדרות עדכון מאפשרות למנהלי מערכת להפעיל או להשבית עדכונים אוטומטיים, להציג או להסתיר את לחצן ' **עדכן כעת** ' ב-Office, לקבוע תאריכי יעד לעדכון ועוד. למידע מפורט, ראו:

- [קביעת תצורה של הגדרות עדכון עבור Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [העדכון האוטומטי עבור Office אינו זמין](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [הגדרת אופן העדכון של Office לאחר התקנתו](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

כדי לסקור את הגדרות העדכונים הקיימים שהוחלו על מחשב לקוח, בצע את הפעולות הבאות:

1. פתח את עורך הרישום על-ידי **הפעלת**  >  **הפעלת**  >  **regedit**.
2. עבור למיקום הבא וסקור את הגדרות Office Update:  
    קצת. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. לחץ על \ קביעת תצורה

**שים לב**  אם המפתח הרפואי מוגדר, ייתכן שתראה את ההודעה "העדכונים מנוהלים על-ידי מנהל המערכת **Office**"  >  **Account**  >  **בעדכונים של office**לחשבון office. לקבלת מידע נוסף, ראה [ניהול עדכונים ל-Microsoft 365 Apps עם מנהל תצורת נקודות הקצה של microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  