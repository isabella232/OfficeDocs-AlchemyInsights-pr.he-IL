---
title: הגדרות מדיניות פגישה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794335"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>ניהול מדיניות פגישה ב-Microsoft Teams

**הערה: אפשרות זו יכולה להימשך עד 24 שעות כדי ששינויי מדיניות ייכנסו לתוקף עבור משתמשים.** ייתכן שלא תוכל לבצע שינויים בפריטי מדיניות חדשים שנוצרו באופן מיידי; המתן 4 שעות ונסה לשנות מדיניות חדשה שנוצרה שוב.

פריטי מדיניות של פגישה משמשים לשליטה בתכונות הזמינות למשתתפים בפגישה לפגישות המתוזמנות על-ידי משתמשים בארגון שלך. ייתכן שתכונות מסוימות של פריטי מדיניות פגישה לא יושמו במרכז הניהול של Teams עדיין (אלה מסומנות "בקרוב" בתיעוד). במקרה זה, או אם אתה מקבל שגיאה כגון "לא ניתן לעדכן את המדיניות כעת, אך נסה שוב מאוחר יותר" במרכז הניהול של Microsoft Teams, מומלץ להשתמש ב-PowerShell כדי ליצור או לשנות מדיניות של פגישות של Teams. 

לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:

- כדי ללמוד אודות יצירת מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה ב-teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- כדי לבצע שינויים במדיניות באמצעות רכיבי cmdlet של PowerShell, ראה [מבט כולל על teams powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - עליך להשתמש במודול מדיניות הפגישה של [Skype For Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) עבור teams. 
    - סקור את [התיעוד של ' רכיבי cmdlet של CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.

