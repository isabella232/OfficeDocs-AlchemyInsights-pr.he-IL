---
title: 'שגיאה: הכללים במחשב זה אינם תואמים'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981114"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>שגיאה: הכללים במחשב זה אינם תואמים

כדי לראות מצב מעודכן של בעיה ידועה זו, ראה [הכללים במחשב זה אינם תואמים לכללים ב- Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

צוות Outlook מיישם תיקון בגיבנה מס' 12928.10000. התיקון כבר נמצא ב- Insider Fast והוא י לעבור לערוץ החודשי בסוף יוני 2020. לאחר שתתקן את ה- Build, ייתכן שתתבקש "אילו כללים ברצונך לשמור" בפעם האחרונה. בחר שרת כאשר תתבקש לעשות זאת ולאחר מכן חזור Outlook ולאחר מכן הפעל מחדש את הכללים שלא היו זמינים.

עד שהתיקון יהיה זמין, השתמש בפתרון הבא:

**פתרון**: בדוחות האחרונים, הבעיה התרחשה עבור אלה שיצרו רק כללי לקוח ב- Outlook שולחן העבודה. אם אתה ממשיך להיכנס לבעיה, שקול למחוק את הכללים ולאחר מכן ליצור ולערוך כללים רק ב- OWA (Outlook Web App) עד לפתרון הבעיה.

אם אין באפשרותך למחוק את הכללים באופן ידני, באפשרותך להפעיל Outlook בעת הפעלת Outlook על-ידי הפעלת Outlook.exe /cleanrules. פעולה זו תמחק הן את כללי הלקוח וגם את כללי השרת. היא תמחק את כל הכללים עבור כל החשבונות בפרופיל Outlook. פקודה זו מתועדת עוד יותר במאמר בוררי שורת הפקודה.

