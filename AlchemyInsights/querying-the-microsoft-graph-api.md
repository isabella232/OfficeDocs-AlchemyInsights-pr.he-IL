---
title: ביצוע שאילתה על ה- API של Microsoft Graph API
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
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923240"
---
# <a name="querying-the-microsoft-graph-api"></a>ביצוע שאילתה על ה- API של Microsoft Graph API

נושא זה עשוי לחול גם על מפתחים שעדיין משתמשים ב- API של Azure AD Graph API. עם זאת, **מומלץ מאוד להשתמש** ב- Microsoft Graph עבור כל תרחישי הניהול של מדריך הכתובות, הזהות והגישה שלך.

**בעיות אימות או מתן הרשאות**

- אם **לאפליקציה** שלך אין אפשרות להשיג אסימונים כדי להתקשר ל- Microsoft Graph, בחר בעיה עם קבלת אסימון גישה **(אימות)** קטגוריית Microsoft Graph כדי לקבל עזרה ותמיכה ספציפיות יותר בנושא זה.
- אם האפליקציה שלך מקבלת שגיאות הרשאה **401 או 403** בעת קריאה ל- Microsoft Graph, בחר את קטגוריית ה- API **של** Microsoft Graph לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.

**אני רוצה להשתמש ב- Microsoft Graph, אך איני בטוח היכן להתחיל**

כדי ללמוד עוד אודות Microsoft Graph, ראה:

- [מבט כולל על Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [מבט כולל על ניהול זהויות Access ב- Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [תחילת העבודה בבניית אפליקציות Microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - בדיקת ממשקי Graph API של Microsoft דייר או דייר הדגמה

**אני רוצה להשתמש ב- Microsoft Graph, אך האם הוא תומך ב- API של מדריך הכתובות v1.0 שאני זקוק לו?**

Microsoft Graph ה- API המומלץ לניהול מדריך כתובות, זהות וגישה. עם זאת, יש עדיין כמה פערים בין מה שניתן ב- Azure AD Graph ו- Microsoft Graph. סקור את המאמרים הבאים, אשר מדגישים את ההבדלים המרובים כדי לסייע בבחירה שלך:

- [הבדלים בין סוגי משאבים בין Azure AD Graph לבין Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [הבדלי המאפיינים בין Azure AD Graph לבין Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [הבדלי שיטה בין Azure AD ל- Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**בעת ביצוע שאילתה *על אובייקט* המשתמש, רבים מהמאפיינים שלו חסרים**

`GET https://graph.microsoft.com/v1.0/users`הפונקציה מחזירה רק 11 מאפיינים, כאשר Microsoft Graph אוטומטית בוחרת ערכת מאפייני משתמש *המהווה ברירת* מחדל להחזרה. אם אתה זקוק *למאפיינים אחרים* של משתמש, השתמש $select כדי לבחור את המאפיינים שהיישום שלך זקוק לו. נסה זאת ב- **Microsoft Graph Explorer תחילה.**

**ערכי המאפיינים של המשתמשים *מסוימים הם Null* למרות שאני יודע שהם מוגדרים**

ההסבר סביר ביותר הוא שהיישום קיבל את ההרשאה *User.ReadBasic.All.* פעולה זו מאפשרת ליישום לקרוא קבוצה מוגבלת של מאפייני משתמש, ומחזירה את כל המאפיינים האחרים כ- Null גם אם הם הוגדרו בעבר. נסה להעניק ליישום את *ההרשאה User.Read.All* במקום זאת.

לקבלת מידע נוסף, ראה [הרשאות משתמש Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**אני נתקל בבעיות בשימוש בפרמטרים של שאילתת OData כדי לסנן נתונים בבקשות שלי**

למרות Graph Microsoft תומך במגוון רחב של פרמטרי שאילתת OData, רבים מפרמטרים אלה אינם נתמכים באופן מלא על-ידי שירותי מדריך כתובות (משאבים היורשים *מ- directoryObject)* ב- Microsoft Graph. אותן מגבלות שהיו קיימים ב- Azure AD Graph עבור רוב מגבלות ב- Microsoft Graph:

1. **לא נתמך**: $count, $search ו- $filter ערכי *Null* *או לא ערכי* Null
2. **לא נתמך**: $filter במאפיינים מסוימים (ראה נושאי משאבים בהם ניתן לסנן מאפיינים)
3. **לא נתמך:** החלפה, סינון ומיון בו-זמנית
4. **לא נתמך**: סינון בקשר גומלין. לדוגמה - מצא את כל החברים בקבוצת ההנדסה שנמצאים בבריטניה.
5. **תמיכה חלקית**: $orderby *המשתמש* (displayName ו- userPrincipalName בלבד) *ובקבוצה*
6. **תמיכה חלקית**: $filter (תומך רק ב- *eq*, *startswith* *,* *או*, ו- , and limited *any*) תמיכה, $expand (הרחבת קשרי גומלין של אובייקט יחיד מחזירה את כל קשרי הגומלין, אך הרחבת אוסף של קשרי גומלין של אובייקטים מוגבלת)

לקבלת מידע נוסף, ראה [התאמה אישית של תגובות באמצעות פרמטרים של שאילתה.](https://docs.microsoft.com/graph/query-parameters)

**ה- API שאני מתקשר אליו אינו פועל - היכן ניתן לעשות בדיקות נוספות?**

**Microsoft Graph Explorer** - בדוק את ממשקי ה Graph API של Microsoft דייר או דייר הדגמה וגם עיין בשאילתות לדוגמה **ב-** Microsoft Graph Explorer.

**כאשר אני מחפש נתונים, נראה שאני מקבל ערכת נתונים לא שלמה בחזרה**

אם אתה עורך שאילתה על אוסף *(כמו* משתמשים), Microsoft Graph משתמש במגבלות עמוד בצד השרת כך שהתוצאות מוחזרות תמיד עם גודל עמוד המוגדר כברירת מחדל. האפליקציה שלך אמורה תמיד לצפות לעבור בין אוספים המוחזרים מהשירות.

לקבלת מידע נוסף, ראה:

- [שיטות עבודה מומלצות Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [החלפת נתוני Graph Microsoft באפליקציה שלך](https://docs.microsoft.com/graph/paging)

**האפליקציה שלי איטית מדי והיא גם מקבלת ויסות. אילו שיפורים ניתן לבצע?**

בהתאם לתרחיש שלך, עומדים לרשותך מגוון אפשרויות שונות כדי להפוך את היישום שלך למבצע יותר, ובתרחישים מסוימים, פחות נוטה ל ויסות על-ידי השירות (כאשר אתה מבצע שיחות רבות מדי).

לקבלת מידע נוסף, ראה:

- [שיטות עבודה מומלצות Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [בקשות אצווה](https://docs.microsoft.com/graph/json-batching)
- [מעקב אחר שינויים באמצעות שאילתת דלתא](https://docs.microsoft.com/graph/delta-query-overview)
- [קבל הודעה על שינויים דרך webhooks](https://docs.microsoft.com/graph/webhooks)
- [הדרכה בנושא ויסות](https://docs.microsoft.com/graph/throttling)

**היכן ניתן למצוא מידע נוסף אודות שגיאות ובעיות ידועות?**

- [מידע Graph של שגיאה של Microsoft](https://docs.microsoft.com/graph/errors)
- [בעיות ידועות ב- Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**היכן ניתן לבדוק את מצב הזמינות והקישוריות של השירות?**

זמינות השירות והקישוריות של השירותים הניתנים לגישה באמצעות Microsoft Graph יכולים להשפיע על הזמינות והביצועים הכוללים של Microsoft Graph.

- עבור תקינות השירות של Azure Active Directory, בדוק את המצב של **שירותי אבטחה + זהות** המפורטים [בדף המצב של Azure](https://azure.microsoft.com/status/).
- לקבלת Office אחרים התורמים ל- Microsoft Graph, בדוק את מצב השירותים המפורטים [בלוח המחוונים Office תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).
