---
title: תיקון מדיניות חיבור
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314845"
---
# <a name="fix-connection-policy"></a>תיקון מדיניות חיבור

הודעת הדואר האלקטרוני סומנה כבטוחה ונמסרה לתיבת הדואר הנכנס של המשתמש מאחר שכתובת ה- IP המהווה מקור סומנה כבטוחה במדיניות מסנן החיבור המוגדרת כברירת מחדל. כדי לסקור את המדיניות, בצע את השלבים הבאים:

1. בפורטל Microsoft 365 Defender ב- , עבור אל מדיניות שיתוף פעולה & דואר אלקטרוני & כללים מדיניות איומים נגד דואר <https://security.microsoft.com/>  \>  \>  \>  זבל **במקטע מדיניות.**

   כדי לעבור ישירות לדף **מדיניות למניעת דואר זבל,** השתמש <https://security.microsoft.com/antispam> ב- .

2. בדף מדיניות למניעת דואר זבל, בחר את המדיניות הנקראת מדיניות מסנן חיבור **(ברירת מחדל)** **על-ידי** לחיצה על שם המדיניות.

3. בתפריט נשלף של הפרטים שמופיע, לחץ **על עריכת מדיניות מסנן חיבור** במקטע **סינון** חיבורים.

4. סקור את הערכים במקטע אפשר **תמיד הודעות מכתובות ה- IP** או מטווח הכתובות הבאים, וסמן אם האפשרות הפעל **רשימה** בטוחה נבחרה.

   **הערה:** Microsoft מנויה למקורות חיצוניים של שולחים מהימנים. אם הרשימה הבטוחה זמינה, שולחים מהימנים אלה אינם מסומנים בטעות כספאם. מומלץ לבחור באפשרות זו, מכיוון שהיא תפחית את מספר חיוביות שגויות (דואר טוב המסווג כסואר זבל) שאתה מקבל.

לקבלת מידע נוסף, ראה [קביעת תצורה של סינון חיבורים](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
