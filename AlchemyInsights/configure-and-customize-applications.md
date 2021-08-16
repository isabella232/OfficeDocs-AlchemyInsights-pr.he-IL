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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044989"
---
# <a name="configure-and-customize-applications"></a>קביעת תצורה והתאמה אישית של יישומים

**קביעת תצורה של יישומים**

1. [התחלה מהירה: קביעת תצורה של מאפיינים עבור יישום בדייר Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) מראה לך כיצד להגדיר חלק מהמאפיינים עבור יישום.
2. כדי לעזור לשלב את היישומים שלך עם Azure Active Directory, פיתחנו [אוסף של ערכות לימוד](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) המסייעות לך לעבור על התצורה.
3. [כיצד להגדיר יישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) עוזר לך להבין כיצד להגדיר יישום Proxy של יישום בתוך Azure AD כדי לחשוף את היישומים המקומיים שלך לענן.
4. [הורד את PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)וקבע את תצורת היישום שלך: בצע את ההוראות בהגדרה *של PingAccess עבור Azure AD* כדי להגן על יישומים שפורסמו באמצעות Microsoft Azure AD Application Proxy באתר האינטרנט Ping Identity והורד את הגירסה העדכנית ביותר של PingAccess.

**שגיאות יישום שגוי (AADSTS650056)**

1. ודא שאתה ניגש ליישום מכתובת הכניסה שסופקה על-ידי הבעלים של היישום. אחרת, היכנס ליישום לאורך התהליך הרגיל שלו. ברוב המקרים פעולה זו תיפתר באופן טבעי. אם לא, פרסום זה יכול לעזור בפתרון בעיות ולפתור אותה.
2. **אם היישום נמצא בבעלות הארגון שלך** (כלומר, רישום היישום נמצא בארגון שלך):
    - לכל הפחות, מומלץ להוסיף את ההרשאה או `User.Read` `openid` **שהוקצתה Graph Microsoft.**
    - ודא שהיישום וכל ההרשאות שלו יתסכימו לכך. באפשרותך לאמת זאת על-ידי **התסת** עמודה רישום היישום בתוך הרשאות **API**.
    - בתרחישים מסוימים, היישום עשוי להיות צד שלישי עם זאת, ייתכן שהוא רשום בארגון שלך. אשר אם יישום זה מופיע ברישום היישומים שלך (יישומים לא ארגוניים).
    - אם אתה ממשיך לראות הודעת שגיאה זו. לאחר מכן, ייתכן שיהיה עליך לבנות את כתובת ה- URL של ההסכמה **המתוארת בשלב 4.**
3. **אם הארגון שלך אינו הבעלים של היישום והשימוש בו כיישום של ספקים אחרים:**
    - אם אתה מנהל המערכת של Global/Company, אתה אמור לראות את מסך ההסכמה. ודא שאתה תבדוק את התיבה **'הסכמה בשם הארגון שלך'.**
    - אם אינך רואה את מסך ההסכמה, מחק את היישום Enterprise ונסה שוב.
    - אם אתה ממשיך לראות הודעת שגיאה זו. לאחר מכן, ייתכן שיהיה עליך לבנות את כתובת ה- URL של ההסכמה **המתוארת בשלב 4.**
4. **בנה באופן ידני את** כתובת ה- URL של ההסכמה לשימוש : אם היישום נועד לגשת למשאב ספציפי, ייתכן שלא תוכל להשתמש בלחצנים הסכמה מפורטל Azure, יהיה עליך ליצור באופן ידני את כתובת ה- URL של הסכמתך ולהשתמש בה.
    - יהיה עליך לקבל את הבעלים `{App-Id}` של `{App-Uri-Id}` היישום ואתו. `{Tenant-Id}` יהיה מזהה הדייר שלך. פעולה זו תהיה או `yourdomain.onmicrosoft.com` מזהה מדריך הכתובות שלך.
    - אם היישום ניגש לעצמו עבור המשאב, הוא יהיה `{App-Id}` `{App-Uri-Id}` זהה.
5. לקבלת מידע נוסף, ראה [בעיות בכניסה ליישומים המוגדרים על-ידי SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)ל כניסה יחידה.

**התאמה אישית של יישומים**

- [הוסף מיתוג לדף](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) הכניסה של Azure Active Directory של הארגון שלך - השתמש בסמל ובערכות צבעים מותאמות אישית של הארגון שלך כדי לספק מראה ורגיש עקבי לדפי הכניסה של Azure Active Directory (Azure AD).
- [הוסף את שם התחום המותאם אישית שלך באמצעות פורטל Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - כל דייר Azure AD חדש מגיע עם שם תחום התחלתי. לא ניתן לשנות או למחוק את שם התחום ההתחלתי, אך באפשרותך להוסיף את שמות הארגון שלך. הוספת שמות תחומים מותאמים אישית עוזרת לך ליצור שמות משתמשים המוכרים למשתמשים שלך.
