---
title: סמל לוח שנה אינו מופיע אצל לקוח Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819954"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>סמל לוח שנה אינו מופיע אצל לקוח Teams

הכרטיסייה 'לוח שנה' ב-Teams מחייבת גישה לתיבת דואר של Exchange דרך Exchange Web Services. תיבת הדואר של Exchange יכול להיות מקוונת או מקומית. עבור משתמשים מקוונים שאין רואים את הכרטיסייה ‘לוח שנה‘, ודא שהם [בעלי רישיון לתיבת דואר של Exchange Online ושתיבת הדואר זמינה](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

אם למשתמש יש תיבת דואר חוקית ב- Exchange Online, אבל הוא עדיין לא יכול לראות את הכרטיסייה ‘לוח שנה‘, ייתכן שאתה נתקל בבעיית רשת. השתמש ב- [מנח הקישוריות המרוחקת של Microsoft](https://testconnectivity.microsoft.com/) והפעל את **בדיקות הקישוריות של שירותי האינטרנט של Microsoft Exchange** עבוד המשתמש המושפע.

לסיום, בדוק את [אפליקציות של Teams - מדיניות הגדרת אפליקציה](https://admin.teams.microsoft.com/policies/app-setup) כדי לוודא שיישום לוח השנה לא הוסר מהמדיניות שחלה על המשתמש (סביר להניח ש **(ברירת המחדל ברחבי הארגון) הכללית**.

אם המשתמשים שלך ממוקמים בבית, עליך לאשר כי קביעת התצורה ההיברידית שלך תקינה. השתמש ב- [אשף קביעת התצורה ההיברידית](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) כדי לפתור בעיות.

שים לב כי [Teams דורש גירסת Exchange 2016 CU3 או גבוהה יותר](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
