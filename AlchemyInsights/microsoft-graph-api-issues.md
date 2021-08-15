---
title: בעיות ב Graph API של Microsoft
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975894"
---
# <a name="microsoft-graph-api-issues"></a>בעיות ב Graph API של Microsoft

נושא זה עשוי לחול גם על מפתחים שעדיין משתמשים ב- API של Azure AD Graph API. עם זאת, **מומלץ מאוד להשתמש** ב- Microsoft Graph עבור כל תרחישי הניהול של מדריך הכתובות, הזהות והגישה שלך.

**בעיות אימות או מתן הרשאות**

- אם **לאפליקציה** שלך אין אפשרות להשיג אסימונים כדי להתקשר ל- Microsoft Graph, בחר בעיה עם קבלת אסימון גישה **(אימות)** קטגוריית Microsoft Graph כדי לקבל עזרה ותמיכה ספציפיות יותר בנושא זה.
- אם האפליקציה שלך מקבלת שגיאות הרשאה **401 או 403** בעת קריאה ל- Microsoft Graph, בחר את קטגוריית ה- API **של** Microsoft Graph לקבל עזרה ותמיכה ספציפיים יותר בנושא זה.

**אני רוצה להשתמש ב- Microsoft Graph, אך איני בטוח היכן להתחיל**

- [מבט כולל על Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [מבט כולל על ניהול זהויות Access ב- Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [תחילת העבודה בבניית אפליקציות Microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - בדיקת ממשקי Graph API של Microsoft דייר או דייר הדגמה

**אני רוצה להשתמש ב- Microsoft Graph, אך האם הוא תומך ב- API של מדריך הכתובות v1.0 שאני זקוק לו?**

Microsoft Graph ה- API המומלץ לניהול מדריך כתובות, זהות וגישה. עם זאת, יש עדיין כמה פערים בין מה שניתן ב- Azure AD Graph ו- Microsoft Graph. סקור את המאמרים הבאים, אשר מדגישים את ההבדלים המרובים כדי לסייע בבחירה שלך:

- [הבדלים בין סוגי משאבים בין Azure AD Graph לבין Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [הבדלי המאפיינים בין Azure AD Graph לבין Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [הבדלי שיטה בין Azure AD ל- Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**ה- API שאני מתקשר אליו אינו פועל - היכן ניתן לעשות בדיקות נוספות?**

**Microsoft Graph Explorer** - בדוק את ממשקי ה Graph API של Microsoft דייר או דייר הדגמה וגם עיין בשאילתות לדוגמה **ב-** Microsoft Graph Explorer.

**האפליקציה שלי איטית מדי והיא גם מקבלת ויסות. אילו שיפורים ניתן לבצע?**

בהתאם לתרחיש שלך, עומדים לרשותך מגוון אפשרויות כדי להפוך את היישום שלך למבצעי יותר, ובתרחישים מסוימים, פחות נוטה להיות ויסות על-ידי השירות (כאשר אתה מבצע שיחות רבות מדי).

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

שגיאות Graph של Microsoft יכולות להיות תוצאה של כמה בעיות שונות, שרובן יוצרות שגיאת 401 או 403. לדוגמה, כל הפעולות הבאות יכולות להוביל לשגיאות מתן הרשאות:

- [זרימות רכישה שגויות של אסימוני גישה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- [טווחי הרשאות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) שתצורתם לא נקבעה כהלכה
- היעדר [הסכמה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***סיום התמיכה עבור Azure Active Directory Authentication Library (ADAL) ו- Azure AD Graph API (AAD Graph)***

**החל מ- 30 ביוני 2020,** לא נוסיף עוד תכונות חדשות לתכונות ADAL ול- Azure AD Graph. נמשיך לספק תמיכה טכנית ועדכוני אבטחה, אך לא נספק עוד עדכוני תכונות.

**החל מ- 30 ביוני 2022,** מסתיים התמיכה ב- ADAL וב- Azure AD Graph ולא תספק עוד תמיכה טכנית או עדכוני אבטחה.

אפליקציות המשתמשות ב- ADAL בגירסאות OS קיימות ימשיכו לפעול לאחר זמן זה, אך לא יתעדכו תמיכה *טכנית או עדכוני אבטחה.*

אפליקציות המשתמשות ב- Azure AD Graph לאחר זמן זה עשויות שלא לקבל עוד תגובות מנקודות הקצה של Azure AD Graph נקודות הקצה.

**ADAL Migration**

אנו ממליצים לעדכן ל[ספריית האימות של Microsoft ‏(MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), הכוללת את התכונות ועדכוני האבטחה האחרונים.

אם אתה משתמש ביישומי Microsoft, תדע ש- Microsoft נמצאת בתהליך העברת היישומים שלה ל- MSAL עד למועד היעד הסופי של התמיכה, כדי להבטיח שהם ייהנו מהאבטחה השוטפת של MSAL ומהשיפורים בתכונה.

1. [קרא את השאלות הנפוצות בנושא ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [למד כיצד להעביר אפליקציות לפי פלטפורמה](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. אם אתה זקוק לעזרה בהבנת אילו מהאפליקציות שלך משתמשות ב- ADAL, מומלץ לסקור את כל קוד המקור של היישומים שלך, ואם ישים, ליצור קשר עם ספקי ISVS או ספקי יישומים. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל האפליקציות שאינן של Microsoft ADAL בדייר שלך.

**העברת AAD Graph**

עבור יישומים המשתמשים ב- Azure AD Graph, בצע את ההנחיות שלנו להעברת [יישומי Azure AD Graph ל- Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [רשימת הפעולות לביצוע של ההעברה מספקת נקודת פתיחה לתחילת העבודה](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. פורטל רישום האפליקציות של Azure מראה אילו אפליקציות משתמשות ב- AAD Graph. אנו ממליצים לך לסקור את קוד המקור של כל האפליקציות שלך, ובמקרה הרלוונטי ליצור קשר עם ISVs או ספקי אפליקציות. התמיכה של Microsoft יכולה גם לספק לך רשימה של כל Graph AAD הדייר שלך.
3. כדי שהאפליקציות שלך לגשת לנתונים ב- Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק לו את ההרשאות הנכונות באמצעות תהליך הסכמה. חומר [ההפניה Graph Microsoft מפרט](https://docs.microsoft.com/graph/permissions-reference) את ההרשאות המשויכות לכל קבוצה ראשית של ממשקי API Graph Microsoft. הוא מספק גם הדרכה לגבי אופן השימוש בהרשאות.
