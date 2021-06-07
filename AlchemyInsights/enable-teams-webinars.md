---
title: הפיכת Teams Webinars לזמינים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793648"
---
# <a name="enable-teams-webinars"></a>הפיכת Teams Webinars לזמינים

Webinars זמינים כברירת מחדל. באפשרותך לנהל מי יכול לתזמן ולרשום Teams Webinars באמצעות Teams PowerShell.

- כל המשתמשים שיכולים ליצור פגישה יכולים גם ליצור פגישת סמינר מקוון. אם ברצונך לנהל מי יכול לתזמן Teams אינטרנט, השתמש *ב- AllowMeetingRegistration*. 
- כברירת מחדל, *WhoCanRegister* זמין ומגדיר **את** כולם. אם ברצונך לבטל את רישום הפגישה, הגדר *את AllowMeetingRegistration ל-* **False**.

כדי לשנות הגדרות אלה, עליך להתקין [את Teams PowerShell](/microsoftteams/teams-powershell-install). כמו כן, מדיניות פגישה נאכפת על-ידי Teams Webinars. לדוגמה, אם ההצטרפות האנונימית מבוטלת בהגדרות הפגישה, משתמשים אנונימיים לא יכולים להצטרף ל- webinars.

לקבלת מידע נוסף על קביעת התצורה של מי יכול להירשם לאתרי אינטרנט, ראה [קביעת תצורה של מי יכול להירשם עבור webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). לקבלת מידע נוסף אודות הגדרות עבור רשימות Microsoft, ראה [הגדרות שליטה עבור רשימות Microsoft.](/sharepoint/control-lists)