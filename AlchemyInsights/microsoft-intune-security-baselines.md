---
title: שימוש Microsoft Intune בסיסי אבטחה כדי לקבוע את התצורה של Windows 10 התקנים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098063"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>שימוש Microsoft Intune בסיסי אבטחה כדי לקבוע את התצורה של Windows 10 התקנים

תוכניות בסיסיות של אבטחה של Intune עוזרות להגן על משתמשים ומכשירים. תוכניות בסיסיות אבטחה הן Windows מוגדרות מראש של קבוצות המשמשות להחלת קבוצה ידועה של הגדרות וערכים המוגדרים כברירת מחדל המומלצים על-ידי צוותי האבטחה הרלוונטיים. על-ידי יצירת פרופיל בסיסי אבטחה ב- Intune, עליך ליצור תבנית המורכבת מפרופילי תצורת מכשיר מרובים.

בעת פריסת תוכניות בסיסיות של אבטחה בקבוצות של משתמשים או מכשירים, ההגדרות מוחלות על מכשירים הפעלה ב- Windows 10 ואילך. לדוגמה, תוכנית הבסיס של ניהול מכשירים ניידים (MDM) של Microsoft מאפשרת באופן אוטומטי את BitLocker עבור כוננים נשלפים, דורשת את הסיסמה לביטול נעילת מכשיר והופכת אימות בסיסי ללא זמין. כאשר ערך ברירת מחדל אינו פועל עבור הסביבה שלך, באפשרותך להתאים אישית את התוכנית הבסיסית כדי להחיל את ההגדרות שאתה זקוק לה.

תוכניות בסיסיות של אבטחה גם עוזרות ליצור זרימת עבודה מאובטחת מ בסוף Microsoft 365. תוכנית בסיסית של אבטחה כוללת את שיטות העבודה המומלצות וההמלצות עבור הגדרות המשפיעות על האבטחה. Intune משתפת קשר עם Windows האבטחה שמיצור תוכניות בסיסיות עבור מדיניות קבוצתית, כך שהמלצות אלה מבוססות על הדרכה מבוססת וניסיון רב.

אם אתה משתמש חדש ב- Intune ולא בטוח היכן להתחיל, תוכניות בסיסיות אבטחה עוזרות לך ליצור ולפרוס במהירות פרופיל מאובטח. אם אתה משתמש כעת במדיניות קבוצתית, המעבר ל- Intune למטרות ניהול קל הרבה יותר עם תוכניות בסיסיות אבטחה מכיוון שהן מוכללות ב- Intune וכוללות יכולות ניהול מתקדמות.

כדי ללמוד עוד, [ראה Windows בסיסי אבטחה וניהול](/windows/security/threat-protection/windows-security-baselines) [מכשירים ניידים](/windows/client-management/mdm/).

