---
title: קביעת התצורה של שירות הסינכרון של MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481874"
---
# <a name="configure-mim-sync-service"></a>קביעת התצורה של שירות הסינכרון של MIM

שירות הסינכרון של Microsoft Identity Manager (MIM) הוא רכיב של MIM. זהו שירות מקומי מרכזי שמאחסן ומשלב מידע עבור ארגונים בעלי ספריות ומסדי נתונים מקומיים מרובים. ייתכן שתוכל לפתור את הבעיה שלך ב-MIM Sync אם הבעיה טופלה בעדכון האחרון ב-MIM או שהיא אחת מהבעיות האחרות המוזכרות בסעיף הבא.

**שלבים מומלצים**

1. ודא שאתה משתמש בעדכון האחרון של MIM Sync ובדוק את [הערות מהדורת הסינכרון של MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) כדי לקבוע אם הבעיה נפתרה בעדכון.
2. אם הבעיה היא באמצעות המחבר הכללי של LDAP, SQL כללי, מחבר לוטוס או מחבר שירותי אינטרנט, ודא שאתה משתמש בעדכון אחרון של [המחברים הכלליים](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. אם מתבצעת הפסקת סינכרון של MIM באמצעות שגיאה, עיין בטבלה של [קודי שגיאה של ההפעלה](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) כדי לקבוע את הסיבות האפשריות.
4. אם ההפעלה מפסיקה עם **סיומת-dll-חריגה** ולאחר מכן לחץ על מילים אלה כדי לפתוח את החלון **מאפיינים של אובייקט מחבר** ולאחר מכן לחץ על **מעקב אחר מחסנית...** כדי לראות מידע נוסף על הסיבה הבסיסית, כפי שמתואר [בהרחבה-dll-חריגה](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. אם השגיאה שינוי סיסמה של שירות ההודעות (PCNS) מדווחת על **שגיאה 6025** ביומן האירועים במהלך סינכרון סיסמאות, סמן את המדריך לפתרון בעיות [בדיווח של PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)ב-6025.
6. אם סינכרון מלא עם סוכן ניהול השירות של FIM מתבצע באיטיות, בדוק את ההגדרה ' **הגדל אוטומטית** ' עבור TempDB, כמתואר [בפתרון בעיות בסינכרון מלא או תלוי](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. אם אתה נתקל בשגיאה של ' הופסק-שרת ' עם כישלון ביצירה-שירותים באינטרנט-שירותים באמצעות הסוכן הניהול של שירות FIM, ראה [תמיכה-מידע: כשל-יצירה-דרך-אינטרנט-שירותים](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) לקבלת מבט כולל על גורמים.

