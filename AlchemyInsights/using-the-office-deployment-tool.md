---
title: שימוש בכלי Office הפריסה
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083771"
---
# <a name="using-the-office-deployment-tool-odt"></a>שימוש בכלי Office (ODT)

השתמש בכלי הפריסה Office (ODT) כדי לפרוס גירסאות Office 365 של Office. כלי Office הפריסה (setup.exe) רץ משורת הפקודה ומשתמש בקובץ XML של תצורה כדי לקבוע אילו הגדרות יש להחיל בעת פריסת Office.
  
1. הורד את הגירסה העדכנית ביותר של כלי Office הפריסה ממרכז [ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. השתמש בכלי [Office אישית (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה וליצור את קובץ ה- XML של התצורה. ייצא את קובץ התצורה ומקום אותו באופן מקומי באותה תיקיה שבה setup.exe שוכנת.

    **הערה:** Office בעיות התקנה נפוצות עקב קבצי תצורה שגויים או קבצי תצורה לא מעוצבים. כדי להימנע מבעיות כאלה, מומלץ להשתמש בכלי ההתאמה האישית Office כדי ליצור את קובץ התצורה. באפשרותך גם לייבא קבצי תצורה קיימים לתוך כלי Office אישית.

3. משורת פקודה עם הרשאות מלאות, עבור למיקום שבו setup.exe נמצא ולהפעיל את כלי הפריסה של Office במצב הורדה וציין את קובץ התצורה שזה עתה שמרת. בדוגמה זו, קובץ התצורה נקרא Configuration.xml:

```setup.exe /download Configuration.xml```

4.הפעל את כלי Office הפריסה במצב קביעת תצורה וציין את קובץ התצורה.

```setup.exe /configure Configuration.xml```

**הערה:** עליך להפעיל שלב זה ממחשב הלקוח שבו ברצונך להתקין את Office ועליה להיות לך הרשאות מנהל מערכת מקומיות במחשב זה.

לקבלת מידע נוסף על השימוש Office פריסה עבור תרחישי הפריסה יישומי Microsoft 365 לארגונים, ראה מבט [כולל על כלי הפריסה של Office הפריסה](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). לקבלת פרטים נוספים אודות אופן השימוש בכלי ההתאמה האישית Office, ראה [מבט כולל על כלי ההתאמה האישית Office שלך](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
