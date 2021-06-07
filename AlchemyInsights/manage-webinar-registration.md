---
title: ניהול רישום סמינר מקוון
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793917"
---
# <a name="manage-webinar-registration"></a>ניהול רישום סמינר מקוון

באפשרותך לנהל מי יכול להירשם Teams Webinars באמצעות Teams Powershell. כדי להתקין Teams Powershell, ראה [Teams PowerShell](/microsoftteams/teams-powershell-install). 

כברירת מחדל, *WhoCanRegister* זמין ומוגדר **ל- EveryoneInCompany**. כדי לאפשר לכל אדם, כולל משתמשים אנונימיים, להירשם, עליך להגדיר את מדיניות **הפגישה** לכולם באמצעות הפקודה Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**הערה**: אם ההצטרפות האנונימית מבוטלת בהגדרות הפגישה, משתמשים אנונימיים לא יכולים להצטרף ל- webinars. כדי ללמוד עוד ולאפשר הגדרה זו, ראה [ניהול הגדרות פגישה ב- Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

אם ברצונך לבטל את רישום הפגישה, הגדר *את AllowMeetingRegistration ל-* **False**.

לקבלת מידע נוסף על קביעת התצורה של מי יכול להירשם לאתרי אינטרנט, ראה [קביעת תצורה של מי יכול להירשם עבור webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). לקבלת מידע נוסף אודות הגדרות עבור רשימות Microsoft, ראה [הגדרות שליטה עבור רשימות Microsoft.](/sharepoint/control-lists)
