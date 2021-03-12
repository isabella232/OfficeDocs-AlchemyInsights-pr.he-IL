---
title: החלת שיטות עבודה מומלצות עבור שאילתות ציד מתקדמות
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746182"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>החלת שיטות עבודה מומלצות עבור שאילתות ציד מתקדמות

כדי לקבל תוצאות במהירות רבה יותר וכדי להימנע מפסקי זמן בעת הפעלת שאילתות מורכבות, החל שיטות עבודה מומלצות אלה:

- בעת ניסיון שאילתות חדשות, השתמש תמיד במגבלה, כדי להימנע מקבלת ערכות תוצאות גדולות מאוד. כמו כן, השתמש `count` כדי לבצע הערכה ראשונית של גודל ערכת התוצאות.
- השתמש תחילה במסנני זמן. באופן אידיאלי, הגבל את השאילתות שלך לשבעה ימים.
- בתחילת שאילתה, מיד לאחר המסנן ' שעה ', הוסף את המסננים הצפויים להסרת רוב הנתונים.
- בעת חיפוש אסימונים מלאים, השתמש `has` באופרטור במקום באופרטור `contains` .
- הפעל חיפוש בעמודה ספציפית במקום בכל העמודות.
- בעת הצטרפות לטבלאות, ציין תחילה את הטבלה עם פחות שורות.
- `project` רק את העמודות הדרושות מהטבלאות שצירפת.

לקבלת מידע נוסף, ראה [שיטות עבודה מומלצות לשאילתות ציד מתקדמות](https://go.microsoft.com/fwlink/?linkid=2144812).
