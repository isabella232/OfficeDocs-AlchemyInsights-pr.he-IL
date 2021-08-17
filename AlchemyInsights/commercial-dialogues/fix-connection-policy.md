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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888407"
---
# <a name="fix-connection-policy"></a>תיקון מדיניות חיבור

הודעת הדואר האלקטרוני סומנה כבטוחה ונמסרה לתיבת הדואר הנכנס של המשתמש מאחר שכתובת ה- IP המהווה מקור סומנה כבטוחה במדיניות מסנן החיבור המוגדרת כברירת מחדל. כדי לסקור את המדיניות, בצע את השלבים הבאים:

1. בפורטל Microsoft 365 Defender ב- , עבור אל מדיניות שיתוף פעולה & דואר אלקטרוני & מדיניות איומים של כללים למניעת דואר <https://security.microsoft.com/>  \>  \>  \>  זבל **במקטע מדיניות.**

   כדי לעבור ישירות לדף **מדיניות למניעת דואר זבל,** השתמש <https://security.microsoft.com/antispam> ב- .

2. בדף מדיניות למניעת דואר זבל, בחר את המדיניות הנקראת מדיניות מסנן חיבור **(ברירת מחדל)** **על-ידי** לחיצה על שם המדיניות.

3. בתפריט נשלף של הפרטים שמופיע, לחץ **על עריכת מדיניות מסנן חיבור** במקטע **סינון** חיבורים.

4. סקור את הערכים במקטע אפשר **תמיד הודעות מכתובות ה- IP** או מטווח הכתובות הבאים, וסמן אם האפשרות הפעל **רשימה** בטוחה נבחרה.

   > [!NOTE]
   > Microsoft מנויה למקורות של ספקים חיצוניים של שולחים מהימנים. אם הרשימה הבטוחה זמינה, שולחים מהימנים אלה אינם מסומנים בטעות כספאם. מומלץ לבחור באפשרות זו, מכיוון שהיא תפחית את מספר חיוביות שגויות (דואר טוב המסווג כסואר זבל) שאתה מקבל.

לקבלת מידע נוסף, ראה [קביעת תצורה של סינון חיבורים](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
