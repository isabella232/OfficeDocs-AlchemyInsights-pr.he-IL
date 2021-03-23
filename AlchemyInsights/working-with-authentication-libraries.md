---
title: עבודה עם ספריות אימות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035831"
---
# <a name="working-with-authentication-libraries"></a>עבודה עם ספריות אימות

כדי לפתור בעיה בספריית האימות של Microsoft (MSAL), בצע את השלבים המומלצים הבאים:

1. **עבודה עם MSAL**: [ספריות אימות של פלטפורמת הזהויות של microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -מאמר זה מציג את התמיכה בספריית האימות של microsoft עבור כמה סוגי יישומים. הוא כולל קישורים לקוד מקור ספריה; היכן לקבל את החבילה עבור הפרוייקט של היישום; והאם הספריה תומכת בכניסה למשתמש (אימות), גישה לממשקי אינטרנט מוגנים (אישור), או שתיהן.

2. **פתרון בעיות באימות**: הMSAL תומך במספר זרימות אימות לשימוש בתרחישים שונים של יישומים. בהתאם לאופן הבנייה של יישום הלקוח שלך, MSAL יכול להשתמש באחד או יותר מזרמי האימות הנתמכים על-ידי פלטפורמת הזהות של Microsoft. זרימות אלה יכולות ליצור מספר סוגים של אסימונים וקודי הרשאות, ולדרוש אסימונים שונים כדי לגרום להם לפעול.

3. **אסימוני גישה**: [אסימוני גישה של פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -למד כיצד ה-API שלך יכול לאמת ולהשתמש בטענות בתוך אסימון גישה. כל התיעוד במאמר זה, למעט היכן שצוין, חל רק על אסימונים שהונפקו עבור APIs שנרשמת. הוא אינו חל על אסימונים שהונפקו עבור ממשקי Api בבעלות Microsoft, וגם לא ניתן להשתמש באסימונים אלה כדי לאמת את האופן שבו פלטפורמת הזהות של Microsoft תיצור אסימונים עבור ממשק API שאתה יוצר.

**סיום התמיכה בספריית האימות של Active Directory (ADAL)**

- **החל מ-30 ביוני, 2020,** לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph. נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.
- **החל מ-30 ביוני 2022,** נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.
- יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא *יקבלו שום תמיכה טכנית או עדכוני אבטחה*.
- יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.

**העברת ADAL**

- מומלץ לעדכן את MSAL, הכולל את התכונות ועדכוני האבטחה העדכניים ביותר.
- אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי מועד היעד של סוף התמיכה, ומבטיחה שייהנו מהאבטחה המתמשכת של MSAL ושיפורים בתכונות.

1. [קרא את השאלות הנפוצות של ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [למד כיצד להעביר אפליקציות על בסיס לכל פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. אם לאחר קריאת המדריך לפלטפורמת האפליקציה שלך, יש לך שאלות נוספות, באפשרותך לפרסם ב- [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) עם התגית [תכלת-ad-adal-תבטלות] או לפתוח בעיה במאגר GitHub של הספריה. עיין במקטע [שפות ומסגרות](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) של מאמר **מבט כולל של MSAL** עבור קישורים לכל מספר ריפו של ספריה.
4. **אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL**, אנו ממליצים לך לסקור את כל קוד המקור של היישומים שלך. במידת הצורך, הושיטו יד לספקי תוכנה עצמאיים (Isv) או לספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.







