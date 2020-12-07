---
title: סמל לוח השנה אינו מוצג בלקוח Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583532"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>סמל לוח השנה אינו מוצג בלקוח Microsoft Teams

הכרטיסיה ' **לוח שנה** ' ב-teams מחייבת גישה לתיבת דואר של exchange באמצעות Exchange Web Services. תיבת הדואר של Exchange יכולה להיות מקוונת או מקומית. עבור משתמשים מקוונים שאינם רואים את הכרטיסיה **לוח שנה** , ודא שהוא [מורשה עבור תיבת דואר של Exchange Online ושתיבת הדואר מאופשרת](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). אם המשתמשים שלך מוצגים באופן מקומי, עליך לוודא שהתצורה ההיברידית שלך בריאה. השתמש ב- [אשף קביעת התצורה ההיברידית](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) כדי לפתור בעיות. שים לב כי [Teams דורש גירסת Exchange 2016 CU3 או גבוהה יותר](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

לקבלת מידע נוסף ושלבי פתרון בעיות, ראה [פתרון בעיות של Microsoft teams ואינטראקציה של Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
