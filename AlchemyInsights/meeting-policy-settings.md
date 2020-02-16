---
title: הגדרות מדיניות פגישה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042845"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>ניהול מדיניות פגישה בצוותי Microsoft

**הערה: ניתן לבצע עד 24 שעות כדי ששינויי מדיניות ייכנסו לתוקף עבור משתמשים.** ייתכן שלא תוכל לבצע שינויים בפריטי מדיניות חדשים שנוצרו באופן מיידי; המתן 4 שעות ונסה לשנות שוב מדיניות חדשה שנוצרה.

מדיניות פגישה משמשת לשליטה בתכונות הזמינות לפגישה עם משתתפים בפגישות שתוזמנו על-ידי משתמשים בארגון שלך. ייתכן שחלק מהתכונות של מדיניות הפגישה לא יושמו במרכז הניהול של הצוותים עדיין (אלה מתויגים "בקרוב" בתיעוד). במקרה זה, או אם אתה מקבל שגיאה כמו "אנחנו לא יכולים לעדכן את המדיניות עכשיו, אבל לנסות את זה שוב מאוחר יותר" במרכז הניהול של צוותי Microsoft, אנו ממליצים להשתמש ב-PowerShell כדי ליצור או לשנות מדיניות פגישה של צוותים. 

לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:

- כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- כדי לבצע שינויי מדיניות באמצעות יישומוני cmdlet PowerShell, ראה [קבוצות מבט כולל של powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - אתה צריך להשתמש [סקייפ עבור עסקים PowerShell מודול](https://www.microsoft.com/download/details.aspx?id=39366) עבור צוותי מדיניות פגישה. 
    - בדוק את [התיעוד *-c, מדיניות יישומוני ה-cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.

