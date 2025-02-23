---
title: שינוי תחום ברירת המחדל של Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950117"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>שינוי תחום ברירת המחדל/הראשי של Yammer

כתובת ה- URL של Yammer מכילה את שם התחום הראשי הנוכחי עבור רשת Yammer שלך. ייתכן ששם תחום זה לא יתאים לשם התחום הראשי שנקבע ב-Office 365 או ב- Azure AD. קיימים הבדלים בהתנהגות בהתבסס על מספר התחומים המותאמים אישית שנוספו לדייר, ואם Yammer מוגדר תחת תצורה נתמכת (דייר 1: רשת 1, או אחד על אחד). תיעוד תחת [תחומים של Yammer ו-Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) זמין.

הסיבה הנפוצה ביותר שבגללה אתה רואה תחום שגוי היא שקיימות רשתות Yammer מרובות ויש לאחד אותן. [איחוד לרשת אחת](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) באמצעות כלי ההעברה של הרשת הוא שלב ראשון חשוב. השלם אותו לפני שתנסה להגדיר את התחום הראשי שלך.

**אין תחומים מותאמים אישית**

עבור דיירים חדשים, תחום ברירת המחדל (לדוגמה fabrikam.onmicrosoft.com) מהדייר ישמש עבור Yammer. התחום הראשי מוגדר אל yammer.com/fabrikam.onmicrosoft.com.

**תחום מותאם אישית יחיד**

Yammer תבחר באופן אוטומטי את תחום ברירת המחדל (לדוגמה fabrikam.com) מהדייר כתחום הראשי ב- Yammer. הוא מוגדר אל yammer.com/fabrikam.com. שינוי זה מבוצע על-ידי שירות סנכרון התחום, ועלול להימשך עד 24 שעות כדי להיכנס לתוקף.

**תחומים מותאמים אישית מרובים**

ל- Yammer יכול להיות תחום ראשי שונה מתחום ברירת המחדל של דייר. מכיוון שיש תחומים מותאמים אישית מרובים, Yammer לא מנסה לנחש את התחום הנכון מבין התחומים הזמינים. עליך לפתוח מקרה תמיכה כדי לבקש לשנו את שם התחום הראשי לתחום הראשי שבחרת.

**מידע נוסף לפתרון בעיות**

במקרים מסומים, ייתכן שתחומים הועברו בין דיירים ולשירות הסנכרון של תחום לא הייתה יכולת לפעול בהצלחה. ייתכן שתחווה בעיות כניסה או בעיות אחרות, בנוסף לתחום ראשי שגוי. כדי לפתור בעיה זו, ייתכן שיהיה להעביר את התחומים אל הרשת הנכונה בעזרת התמיכה של Microsoft. פתרון זה דורש סיוע ישיר ועשוי להימשך זמן מה, במיוחד אם יש רשימת ארוכה מאוד של שמות תחומים. פתח מקרה תמיכה כדי לקבל סיוע בפתרון של סוגי בעיות אלה.

בעת עבודה עם נציג תמיכה, הוא יבדוק שהתחומים מאומתים בדייר תחת שליטתך. ייתכן שהוא ישאל שאלות אימות נוספות בנוגע לתחומים שלך אם הם נוספים לדייר שלך אך אינם מאומתים על-ידי DNS. ודא שהתחומים מאומתים על-ידי DNS כדי לזרז את התהליך.
