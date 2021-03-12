---
title: בעיות API של Microsoft Graph
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713704"
---
# <a name="microsoft-graph-api-issues"></a>בעיות API של Microsoft Graph

נושא זה עשוי גם לחול על מפתחים שעדיין משתמשים ב-API של הודעות מיידיות של גרף. עם זאת, מומלץ **מאוד** להשתמש ב-Microsoft Graph עבור כל תרחישי הספריה, הזהות וניהול הגישה שלך.

**בעיות אימות או הרשאה**

- אם היישום שלך אינו **מצליח לרכוש אסימונים** לצורך התקשרות ל-microsoft graph, בחר **בעיה בקבלת הקטגוריה ' אסימון גישה ' (אימות)** microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.
- אם האפליקציה שלך **מקבלת שגיאות הרשאה של 401 או 403** בעת התקשרות ל-microsoft graph, בחר את הקטגוריה **קבלת שגיאה של microsoft graph שנדחתה (הרשאה)** של microsoft graph כדי לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.

**אני מעוניין להשתמש ב-Microsoft Graph, אך לא בטוח היכן להתחיל**

- [מבט כולל על Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [מבט כולל על זהות וניהול גישה ב-Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [תחילת הבנייה של יישומי Microsoft Graph](https://docs.microsoft.com/graph/)
- **סייר Microsoft graph** -בדיקת ממשקי Api של microsoft graph בדייר שלך או בדייר הדגמה

**אני מעוניין להשתמש ב-Microsoft Graph, אך האם היא תומכת בממשקי Api של מדריכי כתובות של v 1.0 שאני זקוק להם?**

Microsoft Graph הוא ה-API המומלץ עבור מדריכי כתובות, זהויות וניהול גישה. עם זאת, עדיין קיימים כמה פערים בין מה שאפשרי באזור התכלת והגרפי של Microsoft Graph. סקור את המאמרים הבאים, אשר מדגישים את ההבדלים העדכניים ביותר כדי לסייע בבחירתך:

- [הבדלים בין סוגי משאבים בין מע וגרף של Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [הבדלים בין המאפיינים של ' תכלת והגרף ' ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [הבדלי שיטות בין תכלת לספירה ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**ממשק ה-API שאני מתקשר אליו אינו פועל-היכן ניתן לבצע בדיקות נוספות?**

**סייר Microsoft graph** -בדוק את ממשקי ה-Api של microsoft graph בדייר שלך או בדייר הדגמה ועיין גם **בשאילתות לדוגמה** ב-Microsoft Graph Explorer.

**האפליקציה שלי איטית מדי והיא מקבלת מצערת גם כן. אילו שיפורים ניתן לעשות?**

בהתאם לתרחיש שלך, קיימות מגוון אפשרויות לשירותך כדי להפוך את היישום שלך לביצועים טובים יותר, ובמקרים מסוימים, להיות פחות מועדים לוויסות השירות (כאשר אתה מבצע שיחות רבות מדי).

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

שגיאות הרשאה של Microsoft Graph עשויות לנבוע ממספר בעיות שונות, שרובו מפיק שגיאת 401 או 403. לדוגמה, הגורמים הבאים יכולים להוביל לשגיאות הרשאה:

- [זרימות רכישה שגויות של אסימוני גישה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- [טווחי הרשאות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) שתצורתם לא נקבעה כהלכה
- היעדר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_סיום התמיכה עבור ספריית האימות של Azure Active Directory ‏(ADAL) ועבור ה- API של Azure AD Graph ‏(AAD Graph)_* _

_ * החל מ-30 ביוני, 2020 * *, לא נוסיף עוד תכונות חדשות לADAL ו-תכלת AD Graph. נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.

**החל מ-30 ביוני 2022**, נסיים את התמיכה ב-ADAL וב-תכלת לספירה והיא לא תספק עוד תמיכה טכנית או עדכוני אבטחה.

יישומים המשתמשים ב-ADAL בגירסאות מערכת הפעלה קיימות ימשיכו לפעול לאחר שעה זו, אך לא *יקבלו שום תמיכה טכנית או עדכוני אבטחה*.

יישומים המשתמשים ב-תכלת AD Graph לאחר שעה זו עשויים לקבל תגובות מנקודת הקצה של הגרף ' תכלת לספירה '.

**העברת ADAL**

אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.

אם אתה משתמש ב-Microsoft apps, דע ש-Microsoft נמצאת בתהליך העברת היישומים שלה ל-MSAL על-ידי תאריך היעד של סיום התמיכה, ומבטיחה שיפיקו תועלת מהשיפורים המתמשכים של האבטחה והתכונות של MSAL.

1. [קרא את השאלות הנפוצות בנושא ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [למד כיצד להעביר אפליקציות לפי פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. אם אתה זקוק לעזרה בהבנת היישומים שבהם אתה משתמש ב-ADAL, אנו ממליצים לך לסקור את כל קוד המקור של היישומים, ובהתאם לצורך, להושיט יד לכל ספקי Isv או יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור יישומים המשתמשים ב-תכלת AD Graph, בצע את ההנחיות שלנו כדי [להעביר את האפליקציות של הודעות מיידיות של התכלת ל-Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת פתיחה לתחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל השימוש בגרף של ה-עמ-שימוש בדייר שלך.
3. כדי שהיישום שלך ייגש לנתונים ב-Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה. [ההפניה להרשאות Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) מפרטת את ההרשאות המשויכות לכל קבוצה עיקרית של ממשקי Api של Microsoft Graph. כמו כן, הוא מספק הנחיות לגבי אופן השימוש בהרשאות.
