---
title: החל שיטות עבודה מומלצות עבור שאילתות ציד מתקדמות
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930134"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>החל שיטות עבודה מומלצות עבור שאילתות ציד מתקדמות

כדי לקבל תוצאות מהר יותר ולהימנע מתדירות זמן קצוב בעת הפעלת שאילתות מורכבות, החל שיטות עבודה מומלצות אלה:

- בעת ניסיון שאילתות חדשות, השתמש תמיד ב מגבלה, כדי להימנע מקבל ערכות תוצאות גדולות במיוחד. כמו כן, `count` השתמש כדי לבצע הערכה ראשונית של גודל ערכת התוצאות.
- השתמש תחילה במסנני זמן. באופן אידיאלי, הגבל את השאילתות לשבעה ימים.
- בתחילת שאילתה, מיד לאחר מסנן הזמן, הוסף את המסננים הצפויים להסרת רוב הנתונים.
- בעת מחפש אסימונים מלאים, השתמש `has` באופרטור במקום `contains` ב- .
- הפעל חיפוש בטבלה ספציפית עמודה על-פני כל העמודות.
- בעת צירוף טבלאות, ציין תחילה את הטבלה עם פחות שורות.
- `project` רק העמודות הדרושות מהטבלאות שהצטרפת אליהן.

כדי ללמוד עוד, ראה שיטות [עבודה מומלצות מתקדמות של שאילתת ציד](https://go.microsoft.com/fwlink/?linkid=2144812).
