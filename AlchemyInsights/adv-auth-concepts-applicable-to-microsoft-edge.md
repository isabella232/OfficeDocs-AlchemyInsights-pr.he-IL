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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398564"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>מושגי אימות מתקדמים החלים על Microsoft Edge

להלן מושגי האימות המתקדמים החלים על Microsoft Edge:

**אימות יזום**

כאשר תפעיל את [המדיניות ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge ינסה לבצע אימות יזום של משתמשים מחוברים באמצעות שירותי Microsoft. במרווחי זמן קבועים, הוא ישתמש בשירות מקוון כדי לבדוק אם יש מניפסט מעודכן המכיל את התצורה השולטת באימות יזום.

יתרונות: אימות יזום מאפשר אימות לשירותים עיקריים, כגון דף הכרטיסיה החדשה של Office. כמו כן, אם Bing משמש כמנוע החיפוש, אימות יזום משפר את הביצועים של שורת הכתובת ומסייע ליצור תוצאות חיפוש מותאמות אישית לצרכי העסק שלך.

**Windows Hello CredUI עבור אימות NTLM**

אם כניסה יחידה (SSO) אינה זמינה כאשר אתר אינטרנט מנסה להיכנס למשתמש באמצעות מנגנון NTLM או משא ומתן, תכונה זו תאפשר למשתמש לשתף את אישורי מערכת ההפעלה עם אתר האינטרנט ולספק את אתגר האימות באמצעות ממשק המשתמש של Windows Hello Cred. זרימת כניסה זו תופיע רק ב- Windows 10 ורק עבור משתמשים שלא מקבלים SSO במהלך NTLM או משא ומתן על אתגר.

**שימוש בסיסמאות שנשמרו כדי להיכנס באופן אוטומטי**

משתמשים השמירה סיסמאות ב- Microsoft Edge יכולים להפוך כניסה אוטומטית לאתרי אינטרנט שבה הם שמרו אישורים. משתמשים יכולים להפעיל או לבטל תכונה זו edge://settings/passwords, ולקבוע את תצורתה במדיניות [מנהל הסיסמאות.](https://go.microsoft.com/fwlink/?linkid=2134622)
