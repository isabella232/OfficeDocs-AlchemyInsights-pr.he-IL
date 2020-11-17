---
title: שימוש בכלי הפריסה של Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085833"
---
# <a name="using-the-office-deployment-tool-odt"></a>שימוש בכלי הפריסה של Office (ODT)

השתמש בכלי הפריסה של Office (ODT) כדי לפרוס גירסאות office 365 של Office. כלי הפריסה של Office (setupodt.exe) מופעל משורת הפקודה ומשתמש בקובץ XML של תצורה כדי לקבוע אילו הגדרות להחיל בעת פריסת Office.
  
1. הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. השתמש [בכלי ההתאמה האישית של Office (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה שלך וליצור את קובץ ה-XML של התצורה. יצא את קובץ התצורה ומקם אותו באופן מקומי באותה תיקיה שבה הsetupodt.exe נמצא.

    **הערה:** בעיות התקנה של Office מתרחשות בדרך כלל עקב קבצי תצורה שתצורתם שגויה או malformatted. כדי למנוע בעיות מסוג זה, מומלץ להשתמש בכלי ההתאמה האישית של Office כדי ליצור את קובץ התצורה. באפשרותך גם לייבא קבצי תצורה קיימים לכלי ההתאמה האישית של Office.

3. מתוך שורת פקודה מוגבהת, עבור למיקום שבו setupodt.exe ממוקם והפעל את כלי הפריסה של Office במצב הורדה וציין את קובץ התצורה ששמרת זה עתה. בדוגמה זו, קובץ התצורה נקרא Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. הפעלת כלי הפריסה של Office במצב קביעת תצורה וציון קובץ התצורה.

```setupodt.exe /configure Configuration.xml```

**הערה:** עליך לבצע שלב זה ממחשב הלקוח שבו ברצונך להתקין את Office ועליך להיות בעל הרשאות מנהל מערכת מקומי במחשב זה.

לקבלת מידע נוסף אודות השימוש בכלי הפריסה של Office עבור יישומי Microsoft 365 עבור תרחישי פריסה ארגוניים, ראה [מבט כולל על כלי הפריסה של office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). לקבלת פרטים נוספים אודות השימוש בכלי ההתאמה האישית של Office, ראה [מבט כולל על כלי ההתאמה האישית של office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
