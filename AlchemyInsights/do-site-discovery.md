---
title: בצעו גילוי אתר
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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693487"
---
# <a name="do-site-discovery"></a>בצעו גילוי אתר

אם הארגון שלך עדיין משתמש ביישומי אינטרנט מדור קודם ובתוכניות לשימוש במצב Internet Explorer (שרוב הלקוחות מבצע), עליך לבצע גילוי אתרים נוסף.

**כבר פרסת גירסה ישנה יותר של Microsoft Edge**

אם כבר הגדרת את רשימת האתרים של הארגון שלך לעבוד עבור הגירסה המורשית של Microsoft Edge, גילוי האתר שלך כמעט מוכן. הדבר היחיד שייתכן שיהיה עליך לעשות הוא להוסיף אתרים נייטרליים.

אתרים נייטרליים הם בדרך כלל אתרים המספקים כניסה יחידה (SSO). אם אתה עובר לאתר נייטרלי מ-Microsoft Edge, ברצונך להישאר ב-Microsoft Edge כדי לבצע אימות. אם אתה עובר לאתר נייטרלי במצב Internet Explorer, ברצונך להישאר במצב Internet Explorer כדי לבצע אימות.

זהה את כל ה-SSO או אתרים נייטרליים אחרים שבהם אתה משתמש והוסף אותם לרשימת האתרים הארגוניים שלך.

**Internet Explorer הוא דפדפן ברירת המחדל שלך**

אם אתה משתמש רק ב-Internet Explorer כעת, ייתכן שלא תדע אילו אתרים שידרגו לתקני אינטרנט מודרניים ושעדיין דורשים את Internet Explorer. תרצה לחפש ולהוסיף אתרים אלה לרשימת האתרים הארגוניים כדי שתוכל להשתמש במצב Internet Explorer בלבד עבור אתרים אלה.

> [!NOTE]
> [גילוי אתר ארגוני](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) מגלה אתרים שעשויים להזדקק למצב Internet Explorer. היא יכולה לאסוף נתונים במחשבים שבהם פועל Windows Internet Explorer 8 באמצעות Internet Explorer 11 ב-Windows 10, Windows 8.1 או Windows 7.

**ניתוח הנתונים**

לאחר שאספת את נתוני האתר, מומלץ לבצע את ארבעת השלבים הבאים כדי לנתח את הנתונים:
1. מיין את הנתונים לפי תחום ולאחר מכן לפי כתובת URL.
2. הגדר את גבולות האפליקציה לקביעת התצורה עבור מצב Internet Explorer. ברצונך לכלול את כל האתרים ופקדי האינטרנט שמגדירים את היישום, אך אין ברצונך לכלול אתרים ופקדים נוספים. אתרים מסוימים עשויים להיות פשוטים כמו *https://contoso.com/app1* בעוד שאחרים עשויים לדרוש ממך להגדיר אתרים ודפים מרובים.
3. בדוק את האפליקציה כדי לוודא שהיא אינה פועלת במקור. אתרים רבים מציעים תוכן מודרני כאשר הם מזהים דפדפן מודרני ומציעים תוכן מדור קודם רק כאשר הם מזהים את Internet Explorer.
4. הוסף את היישום לרשימת האתרים הארגוניים שלך אם הוא נכשל בבדיקה.

> [!NOTE]
> כשיטת עבודה מומלצת, קבץ את כל האתרים המרכיבים יישום. בדרך זו, בעת שדרוג יישום, קל יותר להסיר את האתר כולו ממצב Internet Explorer ולהתחיל להשתמש בדפדפן מודרני עבור יישום זה.

לאחר שתסיים את גילוי האתר וניתחת את הנתונים, אתה מוכן להתחיל להסתכל על אסטרטגיית הערוץ שלך.

