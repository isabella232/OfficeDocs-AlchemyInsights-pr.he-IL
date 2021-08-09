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
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934366"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>מושגי אימות מתקדמים החלים על Microsoft Edge

להלן מושגי האימות המתקדמים החלים על Microsoft Edge:

**אימות יזום**

כאשר תפעיל את [המדיניות ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge תנסה לבצע אימות יזום של משתמשים מחוברים באמצעות שירותי Microsoft. במרווחי זמן קבועים, הוא ישתמש בשירות מקוון כדי לבדוק אם יש מניפסט מעודכן המכיל את התצורה השולטת באימות יזום.

יתרונות: אימות יזום מאפשר אימות לשירותים עיקריים, כגון Office חדש של כרטיסיה. כמו כן, Bing משמש כמנוע החיפוש, אימות יזום משפר את הביצועים של שורת הכתובת, מסייע ליצור תוצאות חיפוש מותאמות אישית לצרכי העסק שלך.

**Windows Hello CredUI עבור אימות NTLM**

אם כניסה יחידה (SSO) אינה זמינה כאשר אתר אינטרנט מנסה להיכנס למשתמש באמצעות מנגנון NTLM או משא ומתן, תכונה זו תאפשר למשתמש לשתף את אישורי מערכת ההפעלה עם אתר האינטרנט ולספק את אתגר האימות באמצעות ממשק המשתמש Windows Hello Cred. זרימת כניסה זו תופיע רק ב- Windows 10 ורק עבור משתמשים שלא מקבלים SSO במהלך NTLM או משא ומתן על אתגר.

**שימוש בסיסמאות שנשמרו כדי להיכנס באופן אוטומטי**

משתמשים השמירה סיסמאות ב- Microsoft Edge יכולים להפוך כניסה אוטומטית לאתרי אינטרנט שבה הם שמרו אישורים. משתמשים יכולים להפעיל או לבטל תכונה זו edge://settings/passwords, ולקבוע את תצורתה במדיניות [מנהל הסיסמאות.](https://go.microsoft.com/fwlink/?linkid=2134622)
