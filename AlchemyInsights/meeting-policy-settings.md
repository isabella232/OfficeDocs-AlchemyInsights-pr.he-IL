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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925166"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>ניהול מדיניות פגישה ב- Microsoft Teams

**הערה: שינויים במדיניות ייכנסו לתוקף עבור המשתמשים עד 24 שעות.** ייתכן שלא תוכל לבצע שינויים במדיניות חדשה שנוצרה באופן מיידי; המתן 4 שעות ותנסי שוב לשנות מדיניות חדשה שנוצרה.

מדיניות פגישה משמשת לשליטה בתכונות הזמינות למשתתפי הפגישה עבור פגישות המתוזמנות על-ידי משתמשים בארגון שלך. ייתכן שתכונות מסוימות של מדיניות פגישה לא יושמו עדיין במרכז הניהול של Teams (תכונות אלה מסומנות כ"בקרוב" בתיעוד). במקרה זה, או אם אתה מקבל שגיאה כמו "אין לנו אפשרות לעדכן את המדיניות כעת, אך נסה אותה שוב מאוחר יותר" במרכז הניהול של Microsoft Teams, מומלץ להשתמש ב- PowerShell כדי ליצור או לשנות מדיניות Teams פגישה. 

לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:

- כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה ב- Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- כדי לבצע שינויי מדיניות באמצעות כלי cmdlet של PowerShell, [ראה Teams PowerShell .](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - עליך להשתמש במודול [Skype for Business PowerShell עבור](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams פגישה. 
    - עיין [בתיעוד ה- cmdlets של *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.

