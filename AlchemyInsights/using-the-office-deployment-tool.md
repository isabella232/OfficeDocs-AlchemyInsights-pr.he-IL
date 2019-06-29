---
title: שימוש בכלי הפריסה של Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365526"
---
# <a name="using-the-office-deployment-tool-odt"></a>שימוש בכלי הפריסה של Office (ODT)

שימוש בכלי הפריסה של Office (ODT) כדי לפרוס גירסאות Office 365 של Office. כלי הפריסה של Office (setup.exe) פועלת מתוך שורת הפקודה ומשתמש קובץ XML תצורה כדי לקבוע אילו הגדרות כדי להחיל בעת פריסת Office.
  
1. הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office דרך [מרכז ההורדות של Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. השתמש [בכלי ההתאמה האישית של Office (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה שלך וליצור קובץ ה-XML של התצורה. ייצוא קובץ התצורה והעבר אותו באופן מקומי באותה תיקיה בה שוכן setup.exe.

    **הערה:** התקנת office בעיות בדרך כלל מתרחשים יעד שתצורתו אינה מוגדרת כראוי או קבצי תצורה של malformatted. כדי להימנע מבעיות מסוג זה, אנו ממליצים להשתמש בכלי ההתאמה האישית של Office כדי ליצור את קובץ התצורה. באפשרותך גם לייבא קבצי תצורה קיימים לתוך כלי ההתאמה האישית של Office.

3. משורת פקודה עם הרשאות מלאות, לעבור אל המיקום בו שוכן setup.exe להפעיל את כלי הפריסה של Office במצב ההורדה וציין את קובץ התצורה שזה עתה שמרת. בדוגמה זו, קובץ התצורה בשם Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. הפעל את כלי הפריסה של Office בתצורה של מצב וציין את קובץ התצורה.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **הערה:** עליך להפעיל את שלב זה מתוך מחשב הלקוח שבו ברצונך להתקין את Office ודרושות לך הרשאות מנהל מערכת מקומי במחשב זה.

כדי ללמוד עוד אודות שימוש בכלי הפריסה של Office עבור Office 365 ProPlus תרחישי הפריסה, ראה [מבט כולל על כלי הפריסה של Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). לקבלת פרטים נוספים על אופן השימוש בכלי ההתאמה האישית של Office, ראה [מבט כולל על כלי ההתאמה האישית של Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
