---
title: שאילתה ב-API של Microsoft Graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974419"
---
# <a name="querying-the-microsoft-graph-api"></a>שאילתה ב-API של Microsoft Graph

נושא זה עשוי גם לחול על מפתחים שעדיין משתמשים ב-API של הודעות מיידיות של גרף. עם זאת, מומלץ **מאוד** להשתמש ב-Microsoft Graph עבור כל תרחישי הספריה, הזהות וניהול הגישה שלך.

**בעיות אימות או הרשאה**

- אם היישום שלך אינו **מצליח לרכוש אסימונים** לצורך התקשרות ל-microsoft graph, בחר **בעיה בקבלת הקטגוריה ' אסימון גישה ' (אימות)** microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.
- אם האפליקציה שלך **מקבלת שגיאות הרשאה של 401 או 403** בעת התקשרות ל-microsoft graph, בחר את הקטגוריה **קבלת שגיאה של microsoft graph שנדחתה (הרשאה)** של microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.

**אני מעוניין להשתמש ב-Microsoft Graph, אך לא בטוח היכן להתחיל**

לקבלת מידע נוסף אודות Microsoft Graph, ראה:

- [מבט כולל על Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [מבט כולל על זהות וניהול גישה ב-Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [תחילת הבנייה של יישומי Microsoft Graph](https://docs.microsoft.com/graph/)
- **סייר Microsoft graph** -בדיקת ממשקי Api של microsoft graph בדייר שלך או בדייר הדגמה

**אני מעוניין להשתמש ב-Microsoft Graph, אך האם היא תומכת בממשקי Api של מדריכי כתובות של v 1.0 שאני זקוק להם?**

Microsoft Graph הוא ה-API המומלץ עבור מדריכי כתובות, זהויות וניהול גישה. עם זאת, עדיין קיימים כמה פערים בין מה שאפשרי באזור התכלת והגרפי של Microsoft Graph. סקור את המאמרים הבאים, אשר מדגישים את ההבדלים העדכניים ביותר כדי לסייע בבחירתך:

- [הבדלים בין סוגי משאבים בין מע וגרף של Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [הבדלים בין המאפיינים של ' תכלת והגרף ' ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [הבדלי שיטות בין תכלת לספירה ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**כאשר אני מבצע שאילתה על אובייקט *המשתמש* , רבים מהמאפיינים שלו חסרים**

`GET https://graph.microsoft.com/v1.0/users` הפונקציה מחזירה רק 11 מאפיינים, מאחר ש-Microsoft Graph בוחר באופן אוטומטי קבוצת מאפיינים של *משתמש* שברצונך להחזיר. אם אתה זקוק למאפייני *משתמש* אחרים, השתמש ב$select כדי לבחור את המאפיינים הדרושים ליישום שלך. נסה זאת **בסייר Microsoft Graph** תחילה.

**ערכי מאפיינים מסוימים של משתמשים הם *null* למרות שאני יודע שהם מוגדרים**

ההסבר הסביר ביותר הוא שהיישום הוענקה *למשתמש. ReadBasic. All* הרשאה. פעולה זו מאפשרת ליישום לקרוא קבוצה מוגבלת של מאפייני משתמש, ולהחזיר את כל המאפיינים האחרים כערכי null גם אם הם הוגדרו בעבר. נסה להעניק *למשתמש היישום. קרא את כל* ההרשאות במקום זאת.

לקבלת מידע נוסף, ראה [הרשאות משתמש של Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**אני נתקל בבעיות בשימוש בפרמטרי שאילתות של OData כדי לסנן נתונים בבקשות שלי**

בעוד ש-Microsoft Graph תומך בטווח רחב של הפרמטרים של שאילתת OData, רבים מהפרמטרים האלה אינם נתמכים באופן מלא על-ידי שירותי מדריך כתובות (משאבים היורשים מ- *directoryObject*) ב-Microsoft Graph. אותן מגבלות שהיו קיימות ב-תכלת AD Graph נמשכות ברוב המקרים ב-Microsoft Graph:

1. **לא נתמך**: $count, $search ו$filter *בערכי null* או *Not null*
2. **לא נתמך**: $filter במאפיינים מסוימים (ראה נושאי משאבים שעליהם ניתן לסנן מאפיינים)
3. **לא נתמך**: קידוד, סינון ומיון בו
4. **לא נתמך**: סינון בקשר גומלין. לדוגמה-חיפוש כל החברים בקבוצת ההנדסה הנמצאים בבריטניה.
5. **תמיכה חלקית**: $orderby ב- *user* (displayName ו-userPrincipalName בלבד) *וקבוצה*
6. **תמיכה חלקית**: $filter (תומך רק ב- *eq*, ב- *startswith* *או* ב- *and* ובתמיכה *מוגבלת)*, $expand (הרחבת קשרי הגומלין של אובייקט יחיד מחזירה את כל קשרי הגומלין, אך הרחבת אוסף של קשרי גומלין היא מוגבלת)

לקבלת מידע נוסף, ראה [התאמה אישית של תגובות באמצעות פרמטרי שאילתה](https://docs.microsoft.com/graph/query-parameters).

**ה-API שאני מתקשר אליו אינו פועל-היכן ניתן לבצע בדיקות נוספות?**

**סייר Microsoft graph** -בדוק את ממשקי ה-Api של microsoft graph בדייר שלך או בדייר הדגמה ועיין גם **בשאילתות לדוגמה** ב-Microsoft Graph Explorer.

**כאשר אני מבצע שאילתה עבור נתונים, נראה שאני מקבל בחזרה הגדרת נתונים לא מלאה**

אם אתה מבצע שאילתה על אוסף (כגון *משתמשים*), Microsoft Graph משתמש במגבלות עמוד בצד השרת, כך שהתוצאות יוחזרו תמיד עם גודל עמוד המוגדר כברירת מחדל. היישום שלך אמור תמיד לצפות לעמוד באמצעות אוספים המוחזרים מהשירות.

לקבלת מידע נוסף, ראה:

- [שיטות העבודה המומלצות של Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [החלפת נתונים של Microsoft Graph באפליקציה](https://docs.microsoft.com/graph/paging)

**האפליקציה שלי איטית מדי והיא מקבלת מצערת גם כן. אילו שיפורים ניתן לעשות?**

בהתאם לתרחיש שלך, קיימות מגוון אפשרויות שונות לרשותכם כדי להפוך את היישום שלך לביצועים טובים יותר, ובמקרים מסוימים, פחות מועדים לשימוש מצערת על-ידי השירות (כאשר אתה מבצע שיחות רבות מדי).

לקבלת מידע נוסף, ראה:

- [שיטות העבודה המומלצות של Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [בקשות לאצווה](https://docs.microsoft.com/graph/json-batching)
- [מעקב אחר שינויים בשאילתת דלתא](https://docs.microsoft.com/graph/delta-query-overview)
- [קבל הודעה על שינויים באמצעות webhooks](https://docs.microsoft.com/graph/webhooks)
- [הדרכה בוויסות](https://docs.microsoft.com/graph/throttling)

**היכן ניתן למצוא מידע נוסף אודות שגיאות ובעיות ידועות?**

- [מידע אודות תגובת השגיאה של Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [בעיות ידועות ב-Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**היכן ניתן לבדוק את מצב הזמינות והקישוריות של שירות?**

זמינות השירות והקישוריות של השירותים המשמשים כבסיס אליהם ניתן לגשת דרך Microsoft Graph יכולה להשפיע על הזמינות והביצועים הכוללים של Microsoft Graph.

- לקבלת התקינות של שירות השירות של Active Directory, בדוק את מצב **האבטחה +** שירותי זהויות המפורטים [בדף ' מצב תכלת](https://azure.microsoft.com/status/)'.
- עבור שירותי Office התורמים ל-Microsoft Graph, בדוק את מצב השירותים המפורטים [בלוח המחוונים של תקינות השירות של Office](https://portal.office.com/adminportal/home#/servicehealth).
