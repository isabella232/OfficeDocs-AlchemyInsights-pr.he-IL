---
title: Intune Wi-Fi פרופילים
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555310"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi פרופילים

יישום מוצלח של קישוריות Wi-Fi עבור לקוחות MDM תלוי בפרופיל שנפרס כראוי, המשקף את הדרישות של תשתית ה-Wi-Fi הארגונית. כדי לסקור את ההגדרות המתאימות עבור פלטפורמות הלקוח שאתה חוקר, ראה: 

[הוסף הגדרות Wi-Fi עבור התקנים המפעילים אנדרואיד ב-Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[הוספת Wi-Fi הגדרות עבור אנדרואיד ארגוני ייעודי התקנים מנוהלים באופן מלא ב-Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[הוספת הגדרות Wi-Fi עבור התקני iOS ו-iPadOS ב-Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[הוסף הגדרות Wi-Fi עבור Windows 10 והתקנים מאוחרים יותר ב-Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[יבא הגדרות Wi-Fi עבור התקני Windows ב-Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**סוגיות נפוצות**

**אני פורס פרופיל Wi-Fi התלוי באישור שנפרס שצוין בפרופיל Wi-Fi. עם זאת, פרופילי התצורה מציגים מצב שגיאה.**

בדוק שההתקן שלך קיבל את האישור.

1. בIntune, עבור אל **כל ההתקנים** ובחר את **תצורת**ההתקן של התקן _ gt_.

2. ודא שכל הפרופילים הצפויים מפורטים ונמצאים במצב מוצלח.

3. עבור פרופיל דמוי אדם, אם יש לך אישורי ביניים בשרשרת האישורים, ודא שהם פרוסים להתקני Android.

    כדי לבדוק את מצב האישור, עבור אל פרופילי **תצורת התקן**  >  **Profiles**  >  **אנדרואיד מאפייני CA בינוניים**  >  **Properties**  >  **אישור מהימן**.

אם תמשיך לראות שגיאות, סקור את ההליכים ואת מקטעי פתרון התקלות. לקבלת מידע נוסף, ראה [סקירה עבור פתרון בעיות של פרופילי אישורים מסוימים של SCEP באמצעות Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**הפרסתי פרופיל Wi-Fi למכשיר. Intune מראה שהיא הצליחה, אך ההתקן אינו מתחבר ל-Wi-Fi.**

מצב מוצלח פירושו שIntune בהצלחה את הפרופיל כפי שהוגדר. עם זאת, ייתכן שתצורות אלה לא יתאימו לדרישות הרשת ו/או האימות שלך. לקבלת פרטים נוספים אודות ניסיון החיבור, סקור יומני רישום בתשתית ובשירות האימות (בבקר נקודת גישה לאינטרנט אלחוטי ובשרת NPS/Radius). ייתכן שיהיה עליך לעבוד עם צוות תשתית הרשת, או בספק ה-Wi-Fi של הספק החיצוני, כדי לאסוף ולסקור יומני רישום.