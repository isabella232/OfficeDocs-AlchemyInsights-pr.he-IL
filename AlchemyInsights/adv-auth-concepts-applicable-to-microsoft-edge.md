---
title: מושגי אימות מתקדמים החלים על Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573397"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>מושגי אימות מתקדמים החלים על Microsoft Edge

להלן מושגי אימות מתקדמים החלים על Microsoft Edge:

**אימות פרואקטיבי**

בעת הפיכת מדיניות [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) לזמינה, Microsoft Edge מנסה לאמת משתמשים בעלי חתימה באופן פרואקטיבי באמצעות microsoft services. במרווחי זמן קבועים, הוא ישתמש בשירות מקוון כדי לחפש מניפסט מעודכן המכיל את התצורה השולטת באימות פרואקטיבי.

תועלת: אימות פרואקטיבי מאפשר אימות לשירותי מפתח, כגון דף הכרטיסיה החדשה של Office. כמו כן, אם Bing משמש כמנגנון החיפוש, האימות הפרואקטיבי משפר את הביצועים של שורת הכתובת ועוזר ליצור תוצאות חיפוש המותאמות אישית לצרכי העסק שלך.

**Windows שלום CredUI עבור אימות NTLM**

אם כניסה יחידה (SSO) אינה זמינה כאשר אתר אינטרנט מנסה להיכנס למשתמש באמצעות מנגנון NTLM או ניהול משא ומתן, תכונה זו מאפשרת למשתמש לשתף את אישורי מערכת ההפעלה עם אתר האינטרנט ולספק את אתגר האימות באמצעות ממשק המשתמש של Windows שלום. זרימת הכניסה מופיעה רק ב-Windows 10 ורק עבור משתמשים שאינם מקבלים את SSO במהלך האתגר של NTLM או ניהול משא ומתן.

**שימוש בסיסמאות שמורות כדי להיכנס באופן אוטומטי**

משתמשים ששומרים סיסמאות ב-Microsoft Edge יכולים לאפשר כניסה אוטומטית לאתרי אינטרנט שבהם הם שמרו אישורים. המשתמשים יכולים להפעיל או לבטל תכונה זו ב-edge://settings/passwords, ובאפשרותך לקבוע את תצורתה במדיניות [מנהל הסיסמאות](https://go.microsoft.com/fwlink/?linkid=2134622) .
