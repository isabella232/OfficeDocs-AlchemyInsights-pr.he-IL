---
title: הגדרות מדיניות פגישה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825444"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>ניהול מדיניות פגישה ב- Microsoft Teams

**הערה: שינויים במדיניות ייכנסו לתוקף עבור המשתמשים עד 24 שעות.** ייתכן שלא תוכל לבצע שינויים במדיניות חדשה שנוצרה באופן מיידי; המתן 4 שעות ותנסי שוב לשנות מדיניות חדשה שנוצרה.

מדיניות פגישה משמשת לשליטה בתכונות הזמינות למשתתפי הפגישה עבור פגישות המתוזמנות על-ידי משתמשים בארגון שלך. ייתכן שתכונות מסוימות של מדיניות פגישה עדיין לא יושמו במרכז הניהול של Teams (אלה מסומנות כ"בקרוב" בתיעוד). במקרה זה, או אם אתה מקבל שגיאה כמו "אין לנו אפשרות לעדכן את המדיניות כעת, אך נסה אותה שוב מאוחר יותר" במרכז הניהול של Microsoft Teams, מומלץ להשתמש ב- PowerShell כדי ליצור או לשנות את מדיניות הפגישה של Teams. 

לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:

- כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה ב- Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- כדי לבצע שינויי מדיניות באמצעות כלי cmdlet של PowerShell, ראה [מבט כולל על Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - עליך להשתמש במודול [Skype for Business PowerShell עבור](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) פריטי מדיניות פגישה של Teams. 
    - עיין [בתיעוד ה- cmdlets של *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.

