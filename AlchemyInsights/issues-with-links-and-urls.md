---
title: בעיות עם קישורים וכתובות Url
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974465"
---
# <a name="issues-with-links-and-urls"></a>בעיות עם קישורים וכתובות Url

ניתוב מחדש של כתובות Url של URI/השב (שני הביטויים הם להחלפה) הם כתובות ה-Url המשמשות את פלטפורמת הזהויות של Microsoft כדי להחזיר אסימונים המבוקשים על-ידי יישום. לקבלת מידע על כתובות Url אלה, עיין במאמרים הבאים:

- [זרימות אימות ותרחישים של יישומים](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -מידע אודות הניתוב מחדש של רכיבי uri בדף **ההרשמה של האפליקציה** עבור כל תרחיש.
- [ניתוב מחדש של הגבלות ומגבלות של כתובות URL של URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**איני יודע כיצד לרשום את כתובת ה-URL הנכונה של URI/השב עבור היישום שלי**

בעת הכניסה באמצעות היישום שאתה מפתח, אם תיבת הדו של הכניסה מציגה את **AADSTS50011: כתובת ה-url שצוינה בבקשה אינה תואמת לכתובות ה-url של התשובה שתצורתן נקבעה עבור היישום <your app ID>**, יהיה עליך להוסיף לרישום היישומים שלך, ה-URI המנתב המשמש את הקוד בבקשת האסימון לפלטפורמת ה

כדי להוסיף כתובת URL של תשובה, עבור אל הכרטיסיה **אימות** בדף **הרישום של היישום** בפורטל תכלת והוסף ערך במקטע **ניתוב מחדש של רכיבי uri** . כתובות Uri של ניתוב מחדש מוקלדות (אינטרנט או מחשב נייד/שולחן עבודה). הערך שעליך להזין תלוי בסוג היישום שאתה בונה, כמתואר להלן:

- עבור יישומים בעלי עמוד אחד ויישומי אינטרנט, כתובת ה-URL של התשובה היא כתובת URL ביישום שלך. ראה [רישום יישומים בעלי עמוד אחד](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) או [רישום יישום web app באמצעות פורטל תכלת](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- עבור יישומי שולחן העבודה, הערך שעליך לבחור תלוי ב:
    - הפלטפורמה (MacOS שונה מ-Windows או Linux)
    - האופן שבו אתה רוכש את האסימון (באופן אינטראקטיבי, עם זרימת קוד מכשיר, עם אימות משולב של Windows [של יווה] או עם שם משתמש/סיסמה).
    לקבלת פרטים, ראה [יישומי שולחן עבודה-רישום יישומים-ניתוב מחדש של URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- עבור אפליקציות למכשירים ניידים, אורי הניתוב מחדש תלוי ב:
    - הפלטפורמה (iOS/Android/UWP)
    - המידע המשמש לבניית האפליקציה שלך, כגון מזהה החבילה ב-iOS, ושם החבילה וקוד ה-hash של החתימה במכשיר Android הרישום של אפליקציית הפורטל תכלת יסייע לך. לקבלת פרטים, ראה [תצורת פלטפורמה וניתוב מחדש של רכיבי uri](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> ממשקי Api של אינטרנט וחלק מהדרכים השקטה של רכישת אסימונים (של יווה ו-username/password) אינם דורשים מחדש URI.

**פרסת את יישום האינטרנט שלי וכאשר אני מבדוק את האפליקציה שנפרסת, אני מקבל הודעת אי התאמה של כתובת url של תשובה**

הוסף רכיבי Uri של ניתוב מחדש עבור כל המיקומים שבהם אתה מפרוס את יישום האינטרנט שלך. לקבלת מידע נוסף, ראה [רישום יישום web app באמצעות פורטל התכלת](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> הוסף את URI לניתוב מחדש עבור מיקום מיד לאחר שפרסת את היישום במיקום זה.

**איני מצליח לרשום מספיק כתובות Url של תשובות**

אתה משתמש ב-ISV וברשותך מספר כתובות ניתוב מחדש לניתוב מחדש עבור כל לקוח שלך. ברצונך להעביר מ-ADAL/תכלת AD v 1.0 ל-MSAL/פלטפורמת הזהויות של Microsoft והגעת [למספר המרבי של רכיבי uri של ניתוב מחדש](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). כדי לפתור זאת, [הוסף מחדש רכיבי uri למנהלי שירות](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) המתאימים לכל אחד מהלקוחות שלך.
