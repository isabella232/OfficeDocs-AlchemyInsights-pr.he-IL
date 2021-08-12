---
title: חריגה ממגבלת הדואר האלקטרוני היומית. זרימת העבודה מושהית.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914652"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>חריגה ממגבלת הדואר האלקטרוני היומית. זרימת העבודה מושהית.

שגיאה זו עשויה להיתקבל בתרחישים הבאים:

- יש לך זרימת עבודה ב- SharePoint Online המשתמשת בסוג פלטפורמת זרימת העבודה SharePoint 2010 או SharePoint 2013.
- זרימת העבודה מוגדרת לשליחת הודעת דואר אלקטרוני מותאמת אישית ליותר מ- 200 משתמשים בכל פעם, יותר מ- 10,000 נמענים ליום, או יותר מ- 30 הודעות לדקה.
- בעת הפעלת זרימת העבודה, הודעת הדואר האלקטרוני אינה נשלחת ואתה מבחין באופן הפעולה הבא:
    - עבור זרימת עבודה המשתמשת בסוג הפלטפורמה SharePoint 2013, אתר את הדף מצב **זרימת** עבודה. בדף 'מצב זרימת עבודה', המצב **הפנימי** מוגדר ל'הופעל' **ובלון** המידע מציג את לא ניתן **לשלוח לנמען**.

כדי לעקוף בעיה זו, קבע את תצורת זרימת העבודה לשליחת הודעות דואר אלקטרוני מבלי לחרוג [Exchange Online השולחים.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) לדוגמה, השתמש בהשהיה בזרימת העבודה, שלח את הדואר האלקטרוני לקבוצת Microsoft 365, לקבוצת תפוצה או לקבוצת אבטחה זמינה בדואר, או שלח את ההודעה לפחות מ- 200 נמענים בכל פעם.


לקבלת מידע נוסף, עיין במאמר [הבא](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>נושאים קשורים
- [יצירת Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ו- Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 