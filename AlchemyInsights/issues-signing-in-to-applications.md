---
title: בעיות בכניסה ליישומים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901033"
---
# <a name="issues-signing-in-to-applications"></a>בעיות בכניסה ליישומים

כדי לזהות את הסיבה או לאבחן בעיות הקשורות לכניסה למשתמש, בצע את השלבים הבאים:

1. הפעל את [אבחון הכניסה](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. אתר את האירוע לניתוח על-ידי הזנת הפרטים הדרושים לך אודות המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.
3. סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואילו פעולות ניתן לבצע כדי לבצע שינויים, אם נדרשים שינויים כלשהם.

להלן כמה בעיות נפוצות שאתה עשוי להיתקל בהן בעת כניסה ליישומים:

1. אתה או המשתמש **השלמת כניסה ל-תכלת AD, אך אתה רואה בקשה בלתי צפויה** -עיין במאמרים [בקשה בלתי צפויה של הסכמה בעת כניסה ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) [ושגיאה בלתי צפויה בעת ביצוע הסכמה ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. אתה או משתמש **נכנסו ישירות ליישום, אך אינך מצליח להיכנס אליו באמצעות deeplink בפורטל המותאם אישית או בלוח הגישה**: ראה [פתרון בעיות בכניסה ליישום מתוך תכלת AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. אתה או משתמש **השלמת כניסה ל-תכלת ad, אך היישום מציג הודעת שגיאה ואינו מאפשר למשתמש לסיים את זרימת הכניסה**: הבעיה היא שהיישום לא קיבל את התגובה שהנפיקה תכלת AD. בצע [שלבים אלה](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) כדי לפתור את הבעיות.
4. אתה או משתמש **לא מצליח להיכנס ליישום שאינו בגלריה שתצורתו נקבעה עבור כניסה יחידה לסיסמאות**: בצע את ההדרכה [בשלבים אלה](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) כדי לפתור את הבעיות.
5. אתה או משתמש **לא מצליח להיכנס ליישום בגלריה ' תכלת והודעות ' שתצורתו נקבעה עבור כניסה יחידה לסיסמאות**: בצע את [השלבים הבאים](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) כדי לפתור בעיות.
6. אתה או משתמש **לא מצליח להיכנס ליישום של Microsoft**: בצע [שלבים אלה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) כדי לפתור את הבעיות.
7. אתה או משתמש **לא מצליח להיכנס ליישום שאינו מהגלריה שתצורתו נקבעה עבור כניסה יחידה מאוחדת**: בצע [שלבים אלה](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) כדי לפתור את הבעיות.
8. אתה או משתמש **לא מצליח להיכנס ליישום בגלריה ' תכלת ולאחר ' שתצורתו נקבעה עבור כניסה יחידה מאוחדת**: בצע [שלבים אלה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) כדי לפתור את הבעיות.
9. אתה או משתמש **לא מצליח להיכנס ליישום מותאם אישית**: בצע [שלבים אלה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) כדי לפתור את הבעיות.
10. אתה או משתמש **לא מצליח להיכנס ליישום מקומי באמצעות ה-proxy של היישום ' תכלת לספירה '**: בצע [שלבים אלה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) כדי לפתור את הבעיות.

