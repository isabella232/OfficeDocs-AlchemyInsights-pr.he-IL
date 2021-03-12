---
title: בעיות באמצעות משאב או מנהל שירות
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713664"
---
# <a name="issues-with-a-resource-or-service-principal"></a>בעיות באמצעות משאב או מנהל שירות

1. אם אתה רק מתחיל בעבודה, [אובייקטים ראשיים של יישומים ושירותים ב-תכלת Active directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) מתאר רישום יישומים, אובייקטי יישומים ומנהלי שירות ב-תכלת active directory: מה הם, כיצד הם משמשים וכיצד הם קשורים זה לזה. תרחיש דוגמה רב-דייר מוצג גם כדי להמחיש את קשרי הגומלין בין אובייקט האפליקציה של יישום לבין אובייקטים ראשיים של שירות.
2. באפשרותך לקבל מידע נוסף אודות קשרי הגומלין בין יישומים ומנהלי שירות על-ידי קריאת [יישומים ואובייקטים ראשיים של שירות ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [כיצד לבצע את הפעולות הבאות: שימוש בפורטל כדי ליצור יישום ומנהל שירות של ' תכלת ושירותים ' שיכולים לגשת למשאבים](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) מראה לך כיצד ליצור יישום חדש של תכלת active Directory (תכלת לספירה) ומנהל שירות שניתן להשתמש בו עם בקרת גישה מבוססת תפקידים.
4. באמצעות ה- [API הראשי של השירות](https://docs.microsoft.com/graph/api/resources/serviceprincipal), באפשרותך לנהל באופן תוכניתי מופעים של יישומים ולשלוט במה שיישום יכול לבצע בתוך הדייר שלך.
5. [סוג המשאב servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) מפרט את כל המאפיינים והשיטות עבור סוג המשאב של servicePrincipal.
6. [הבדלים בסוגי משאבים בין כגון תכלת לגרף ו-Microsoft graph מדגיש את ההבדלים](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) בין מקורות התכלת והגרף של משאבי microsoft graph. היא מציגה משאבים בעלי שמות שונים או אינם זמינים; היא גם מסמנת משאבים הזמינים בגירסת הביתא של Microsoft Graph, אך לא בגירסת v 1.0.

**בעיות עם משתמשים אורחים**

- [תחלה: הוספת משתמשי אורח למדריך הכתובות בפורטל תכלת](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) מראה לך כיצד להוסיף משתמש אורח חדש למדריך הכתובות של התכלת באמצעות פורטל תכלת, לשלוח הזמנה ולראות איך נראה תהליך החזרת ההזמנה של המשתמש אורח.
- [ערכת לימוד: יצירת זרמי משתמשים ב-תכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) מראה לך כיצד ליצור זרימות מומלצות של משתמשים מומלצים באמצעות הפורטל ' תכלת '. אם אתה מחפש מידע אודות אופן הגדרת הזרימה של אישורי סיסמה של בעלי משאב (ROPC) ביישום שלך, ראה קביעת התצורה של זרימת אישורי הסיסמה של בעלי המשאב בתכלת AD B2C.
