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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794912"
---
# <a name="using-the-office-deployment-tool-odt"></a>שימוש בכלי הפריסה של Office (ODT)

השתמש בכלי הפריסה של Office (ODT) כדי לפרוס גירסאות office 365 של Office. כלי הפריסה של Office ( setup.exe ) מופעל משורת הפקודה ומשתמש בקובץ XML של תצורה כדי לקבוע אילו הגדרות להחיל בעת פריסת Office.
  
1. הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. השתמש [בכלי ההתאמה האישית של Office (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה שלך וליצור את קובץ ה-XML של התצורה. יצא את קובץ התצורה ומקם אותו באופן מקומי באותה תיקיה שבה החנות setup.exe נמצאת.

    **הערה:** בעיות התקנה של Office מתרחשות בדרך כלל עקב קבצי תצורה שתצורתם שגויה או malformatted. כדי למנוע בעיות מסוג זה, מומלץ להשתמש בכלי ההתאמה האישית של Office כדי ליצור את קובץ התצורה. באפשרותך גם לייבא קבצי תצורה קיימים לכלי ההתאמה האישית של Office.

3. מתוך שורת פקודה מוגבהת, עבור למיקום שבו הוא setup.exe נמצא והפעל את כלי הפריסה של Office במצב הורדה וציין את קובץ התצורה ששמרת זה עתה. בדוגמה זו, קובץ התצורה נקרא Configuration.xml :

```setup.exe /download Configuration.xml```

4. הפעלת כלי הפריסה של Office במצב קביעת תצורה וציון קובץ התצורה.

```setup.exe /configure Configuration.xml```

**הערה:** עליך לבצע שלב זה ממחשב הלקוח שבו ברצונך להתקין את Office ועליך להיות בעל הרשאות מנהל מערכת מקומי במחשב זה.

לקבלת מידע נוסף אודות השימוש בכלי הפריסה של Office עבור יישומי Microsoft 365 עבור תרחישי פריסה ארגוניים, ראה [מבט כולל על כלי הפריסה של office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). לקבלת פרטים נוספים אודות השימוש בכלי ההתאמה האישית של Office, ראה [מבט כולל על כלי ההתאמה האישית של office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
