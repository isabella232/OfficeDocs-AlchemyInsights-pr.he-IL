---
title: קביעת תצורה והתאמה אישית של יישומים
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063620"
---
# <a name="configure-and-customize-applications"></a>קביעת תצורה והתאמה אישית של יישומים

**קביעת תצורה של יישומים**

1. [תחלה: קביעת תצורה של מאפיינים עבור יישום בדייר תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) מראה לך כיצד לקבוע את התצורה של חלק מהמאפיינים עבור יישום.
2. כדי לעזור לשלב את היישומים שלך ב-תכלת Active Directory, פיתחנו [אוסף של ערכות לימוד](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) שיובילו אותך באמצעות התצורה.
3. [כיצד לקבוע תצורה של יישום proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) מסייע לך להבין כיצד להגדיר יישום Proxy של יישום בתוך תכלת לספירה כדי לחשוף את היישומים המקומיים שלך לענן.
4. [הורד את PingAccess וקבע את התצורה של היישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): בצע את ההוראות במאמר *קביעת התצורה של PingAccess עבור תכלת לספירה כדי להגן על יישומים* שפורסמו באמצעות היישום Proxy של Microsoft הודעות מיידיות באתר האינטרנט של Ping Identity והורד את הגירסה העדכנית

**שגיאות יישום שתצורתן הוגדרו (AADSTS650056)**

1. ודא שאתה ניגש ליישום מכתובת הכניסה שמספקת בעלי היישום. אחרת, היכנס ליישום באמצעות התהליך הרגיל שלו. ברוב המקרים, פעולה זו תיפתר באופן אוטומטי. אם היא אינה מופיעה, רשומה זו יכולה לעזור לפתור את הבעיה ולפתור אותה.
2. **אם לארגון שלך יש את היישום** (כלומר, רישום היישום נמצא בארגון שלך):
    - לכל הפחות, מומלץ `User.Read` `openid` להוסיף את ההרשאה או הנציגה מ- **Microsoft Graph** .
    - ודא שהיישום וכל ההרשאות שלו מסכימים לכך. באפשרותך לאמת זאת על-ידי התבוננות בעמודה **מצב** של רישום היישום בתוך **הרשאות API**.
    - בתרחישים מסוימים, היישום עשוי להיות צד שלישי, אולם ייתכן שהוא יירשם בארגון שלך. אשר אם יישום זה מופיע ברישומי היישומים שלך (לא ביישומים ארגוניים).
    - אם תמשיך לראות הודעת שגיאה זו. לאחר מכן ייתכן שתצטרך לבנות את כתובת ה-URL של ההסכמה המתוארת **בשלב 4**.
3. **אם הארגון שלך אינו הבעלים של היישום ומשתמש בו כיישום של ספק חיצוני**:
    - אם אתה מנהל המערכת הכללי/החברה, אתה אמור לראות את המסך ההסכמה. הקפד לסמן את התיבה **"הסכמה בשם הארגון שלך"**.
    - אם אינך רואה את המסך ' הסכמה ', מחק את יישום הארגון ונסה שוב.
    - אם תמשיך לראות הודעת שגיאה זו. לאחר מכן ייתכן שתצטרך לבנות את כתובת ה-URL של ההסכמה המתוארת **בשלב 4**.
4. **בניית כתובת ה-url המתקבלת באופן ידני**: אם היישום מיועד לגשת למשאב ספציפי, ייתכן שלא תוכל להשתמש בלחצני ההסכמה מפורטל התכלת, יהיה עליך ליצור באופן ידני את כתובת ה-url המתקבלת שלך ולהשתמש באפשרות זו.
    - יהיה עליך להשיג את `{App-Id}` `{App-Uri-Id}` הבעלים של היישום וממנו. `{Tenant-Id}` יהיה מזהה הדייר שלך. פעולה זו תהיה `yourdomain.onmicrosoft.com` או מזהה מדריך הכתובות שלך.
    - אם היישום ניגש לעצמו עבור המשאב, אזי ה `{App-Id}` `{App-Uri-Id}` -and יהיה זהה.
5. לקבלת מידע נוסף, ראה [בעיות בכניסה ליישומים המוגדרים כניסה יחידה מבוססת SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**התאמה אישית של יישומים**

- [הוספת מיתוג לעמוד הכניסה של הארגון תכלת Active directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) -השתמש בסמל הארגון שלך ובערכות צבעים מותאמות אישית כדי לספק מראה עקבי ומבט עקבי לעמודי הכניסה של תכלת active Directory (תכלת לספירה).
- [הוסף את שם התחום המותאם אישית שלך באמצעות פורטל ' תכלת Active Directory '](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) -כל דייר חדש של ' תכלת הפרסומות ' מגיע עם שם תחום ראשוני. לא ניתן לשנות או למחוק את שם התחום ההתחלתי, אך באפשרותך להוסיף את שמות הארגון שלך. הוספת שמות תחומים מותאמים אישית עוזרת לך ליצור שמות משתמשים המוכרים למשתמשים שלך.
