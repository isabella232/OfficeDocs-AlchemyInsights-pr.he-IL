---
title: שימוש בכלי הפריסה של Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010867"
---
# <a name="using-the-office-deployment-tool-odt"></a>שימוש בכלי הפריסה של Office (ODT)

השתמש בכלי הפריסה של Office (ODT) כדי לפרוס גירסאות office 365 של Office. כלי הפריסה של Office (setup. exe) מופעל מתוך שורת הפקודה ומשתמש בקובץ XML של תצורה כדי לקבוע אילו הגדרות יחולו בעת פריסת Office.
  
1. הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. השתמש [בכלי התאמה אישית של Office (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה שלך וליצור את קובץ ה-XML של התצורה. יצא את קובץ התצורה ומלא אותו באופן מקומי באותה תיקייה שבה נמצאת ההתקנה. exe.

    **הערה:** בעיות התקנה של Office מתרחשות בדרך כלל עקב קבצי תצורה שאינם מאותחלים או מעוצבים. כדי להימנע מבעיות כאלה, מומלץ להשתמש בכלי ההתאמה האישית של Office כדי ליצור את קובץ התצורה. באפשרותך גם לייבא קבצי תצורה קיימים לכלי ההתאמה האישית של Office.

3. משורת פקודה עם הרשאות מלאות, עבור למיקום שבו setup. exe שוכן והפעל את כלי הפריסה של Office במצב הורדה וציין את קובץ התצורה ששמרת זה עתה. בדוגמה זו, קובץ התצורה נקרא תצורה. xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. הפעל את כלי הפריסה של Office במצב קביעת תצורה וציין את קובץ התצורה.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **הערה:** עליך להפעיל שלב זה ממחשב הלקוח שבו ברצונך להתקין את Office ועליך להיות בעל הרשאות מנהל מקומיות במחשב זה.

כדי ללמוד עוד אודות השימוש בכלי פריסת Office עבור יישומי Microsoft 365 עבור תרחישי פריסה ארגוניים, ראה [מבט כולל על כלי הפריסה של office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). לקבלת פרטים נוספים על אופן השימוש בכלי ההתאמה האישית של Office, ראה [מבט כולל על כלי ההתאמה האישית של office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
