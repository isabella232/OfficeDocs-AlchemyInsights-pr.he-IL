---
title: בעיות בקישורים ובכתובות URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054799"
---
# <a name="issues-with-links-and-urls"></a>בעיות בקישורים ובכתובות URL

URI של ניתוב מחדש/כתובות URL של תשובה (לא ניתן להחליף בין שני הביטויים) הן כתובות ה- URL שנמצאות בשימוש על-ידי פלטפורמת הזהויות של Microsoft כדי להחזיר אסימונים שהתבקשו על-ידי האפליקציה. לקבלת מידע על כתובות URL אלה, עיין במאמרים הבאים:

- [זרימות אימות ותרחישי אפליקציות](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - מידע על כתובות ה- URL של משתני URI של ניתוב מחדש דף **רישום אפליקציה** עבור כל תרחיש.
- [הגבלות ומגבלות של ניתוב מחדש של URI/כתובת URL של תשובה](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**איני יודע כיצד לרשום את URI של ניתוב מחדש / כתובת URL של תשובה עבור האפליקציה שלי**

בעת הכניסה באמצעות האפליקציה שאתה מפתח, אם תיבת הדו-שיח של הכניסה מציגה **AADSTS50011: כתובת ה- URL של התשובה שצוינה בבקשה אינה תואמת לכתובות ה- URL של התשובה שהוגדרו עבור האפליקציה <your app ID>**, יהיה עליך להוסיף לרישום האפליקציות שלך, את ה- URI לניתוב מחדש שבו הקוד שלך השתמש בבקשה לאסימון אל פלטפורמת הזהויות של Microsoft.

כדי להוסיף כתובת URL של תשובה, עבור אל הכרטיסיה **אימות** בדף **רישום אפליקציות** בפורטל Azure והוסף הזנה במקטע **משתני URI של ניתוב מחדש**. הערך שאתה צריך להזין תלוי בסוג האפליקציה שאתה בונה, כמתואר להלן:

- עבור אפליקציות בדף בודד ואפליקציות אינטרנט, כתובת ה- URL של התשובה היא כתובת URL באפליקציה שלך. ראה [רישום אפליקציות בדף אחד](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) או [רישום אפליקציית אינטרנט באמצעות פורטל Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- עבור אפליקציות שולחן העבודה, הערך שיש לבחור תלוי ב:
    - הפלטפורמה (MacOS שונה מ- Windows או מ- Windows)
    - האופן שבו נרכש האסימון (באופן אינטראקטיבי, עם זרימת קוד מכשיר, עם אימות משולב של אימות Windows [IWA] אן עם שם משתמש/סיסמה).
    לקבלת פרטים, ראה [אפליקציות שולחן עבודה - רישום אפליקציה - URi של ניתוב מחדש](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- עבור אפליקציות למכשירים ניידים, ה- URI של ניתוב מחדש תלוי ב:
    - בפלטפורמה (iOS/Android/UWP)
    - במידע המשמש לבניית האפליקציה שלך, כגון מזהה החבילה ב- iOS, ו- Hash של שם החבילה והחתימה ב- Android, רישום האפליקציה בפורטל Azure יעזור לך. לקבלת פרטים, ראה [קביעת התצורה של הפלטפורמה ומשתני URI של ניתוב מחדש](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> ממשקי API של אינטרנט וחלק מהדרכים השקטות לרכישת אסימונים (IWA ושם משתמש/סיסמה) אינם דורשים URI של ניתוב מחדש.

**פרסתי את אפליקציה האינטרנט שלי וכשאני בודק את האפליקציה שנפרסה, אני מקבל הודעה על אי-התאמה של כתובת URL של תשובה**

הוסף URI של ניתוב מחדש עבור כל המיקומים שבהם אתה פורס את אפליקציית האינטרנט. לקבלת מידע נוסף, ראה [רשום אפליקציית אינטרנט באמצעות פורטל Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> הוסף URI של ניתוב מחדש עבור מיקום מיד לאחר שפרסת את האפליקציה במיקום זה.

**איני יכול לרשום מספיק כתובות URL של תשובה**

אתה ספק תוכנה עצמאי ויש לך כתובת URL אחת או כמה כתובות URL של ניתוב מחדש עבור כל לקוח שלך. ברצונך לבצע העברה מ- ADAL/Azure AD v1.0 ל- MSAL/פלטפורמת הזהויות של Microsoft [מספר מקסימלי של משתני URL של ניתוב מחדש](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). כדי לפתור בעיה זו, [הוסף משתני URI של ניתוב מחדש לעקרונות שירות](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) שתואמים לכל אחד מהלקוחות שלך.
