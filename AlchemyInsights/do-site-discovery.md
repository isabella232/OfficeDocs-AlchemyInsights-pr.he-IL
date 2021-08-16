---
title: האם גילוי אתר
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030759"
---
# <a name="do-site-discovery"></a>האם גילוי אתר

אם הארגון שלך עדיין משתמש באפליקציות אינטרנט מדור קודם ובתוכניות לשימוש במצב Internet Explorer (שרוב הלקוחות עושים זאת), עליך לעשות גילוי אתר נוסף.

**כבר פרסת גירסה קודמת של Microsoft Edge**

אם כבר הגדרת את רשימת האתרים הארגוניים שלך כך שתעבד עבור הגירסה מדור קודם של Microsoft Edge, גילוי האתר שלך כמעט מוכן. הדבר היחיד שייתכן שתצטרך לעשות הוא להוסיף אתרים ניטרליים.

אתרים ניטרליים הם בדרך כלל אתרים המספקים כניסה יחידה (SSO). אם אתה הולך לאתר ניטרלי Microsoft Edge, ברצונך להישאר Microsoft Edge לאמת. אם אתה הולך לאתר ניטרלי במצב Internet Explorer, ברצונך להישאר במצב Internet Explorer כדי לבצע אימות.

זהה כל SSO או אתרים ניטרליים אחרים שאתה משתמש בהם והוסף אותם לרשימת האתרים הארגוניים שלך.

**Internet Explorer הוא דפדפן ברירת המחדל שלך**

אם אתה משתמש ב- Internet Explorer רק כעת, ייתכן שלא תדע אילו אתרים שדרגו לתקני אינטרנט מודרניים ותידרש עדיין את Internet Explorer. תרצה למצוא ולהוסיף אתרים אלה לרשימת האתרים הארגוניים כדי שתוכל להשתמש במצב Internet Explorer רק עבור אתרים אלה.

> [!NOTE]
> [גילוי אתר ארגוני מגלה](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) אתרים שייתכן שתצטרך את מצב Internet Explorer. הוא יכול לאסוף נתונים במחשבים שבהם פועל Internet Explorer 8 Windows Internet Explorer 11 ב- Windows 10, Windows 8.1 או Windows 7.

**ניתוח הנתונים**

לאחר איסוף נתוני האתר, מומלץ לבצע את התהליך בן ארבעת השלבים הבאים כדי לנתח את הנתונים:
1. מיין את הנתונים לפי תחום ולאחר מכן לפי כתובת URL.
2. הגדר את הגבולות של יישום כדי לקבוע את תצורתו עבור מצב Internet Explorer. ברצונך לכלול את כל האתרים ופקדי האינטרנט המגדירים את היישום, אך אינך מעוניין לכלול אתרים ופקדים נוספים. אתרים מסוימים עשויים להיות פשוטים *https://contoso.com/app1* כמו שאחרים עשויים לדרוש ממך להגדיר אתרים ודפים מרובים.
3. בדוק את היישום כדי לוודא שהוא אינו פועל באופן מקורי. אתרים רבים מציעים תוכן מודרני כאשר הם מזהים דפדפן מודרני ומציעים תוכן מדור קודם רק כאשר הם מזהים את Internet Explorer.
4. הוסף את היישום לרשימת האתרים הארגוניים שלך אם הוא נכשל בבדיקה.

> [!NOTE]
> כשיטות עבודה מומלצות, קבץ את כל האתרים המורכבים מיישום. בדרך זו, בעת שדרוג יישום, קל יותר להסיר את האתר כולו ממצב Internet Explorer ולהתחיל להשתמש בדפדפן מודרני עבור יישום זה.

לאחר סיימת עם גילוי האתר ותנתח את הנתונים, אתה מוכן להתחיל לבחון את אסטרטגיית הערוץ שלך.

