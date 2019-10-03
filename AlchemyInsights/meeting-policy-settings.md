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
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376664"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>ניהול מדיניות פגישה בצוותי Microsoft

מדיניות פגישה משמשת לשליטה בתכונות הזמינות לפגישה עם משתתפים בפגישות שתוזמנו על-ידי משתמשים בארגון שלך. ייתכן שחלק מהתכונות של מדיניות הפגישה לא יושמו במרכז הניהול של הצוותים עדיין (אלה מתויגים "בקרוב" בתיעוד). במקרה זה, או אם אתה מקבל שגיאה כמו "אנחנו לא יכולים לעדכן את המדיניות עכשיו, אבל לנסות את זה שוב מאוחר יותר" במרכז הניהול של צוותי Microsoft, אנו ממליצים להשתמש ב-PowerShell כדי ליצור או לשנות מדיניות פגישה של צוותים. 

לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:

- כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- כדי לבצע שינויי מדיניות באמצעות יישומוני cmdlet PowerShell, ראה [קבוצות מבט כולל של powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - אתה צריך להשתמש [סקייפ עבור עסקים PowerShell מודול](https://www.microsoft.com/download/details.aspx?id=39366) עבור צוותי מדיניות פגישה. 
    - בדוק את [התיעוד *-c, מדיניות יישומוני ה-cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.

**הערה:** זה יכול להימשך עד 24 שעות כדי שהשינויים במדיניות ייכנסו לתוקף עבור משתמשים. ייתכן שלא תוכל לבצע שינויים בפריטי מדיניות חדשים שנוצרו באופן מיידי; המתן 4 שעות ונסה לשנות שוב מדיניות חדשה שנוצרה. אם עדיין יש לך בעיות, נסה PowerShell.  