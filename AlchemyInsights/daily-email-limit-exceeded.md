---
title: אירעה חריגה ממגבלת הדואר האלקטרוני היומית. זרימת העבודה מושעית.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053118"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>אירעה חריגה ממגבלת הדואר האלקטרוני היומית. זרימת העבודה מושעית.

שגיאה זו עשויה להתקבל בתרחישים הבאים:

- ברשותך זרימת עבודה ב-SharePoint Online המשתמשת בסוג פלטפורמת זרימת העבודה sharepoint 2010 או SharePoint 2013.
- תצורת זרימת העבודה מוגדרת לשליחת הודעת דואר אלקטרוני מותאמת אישית ליותר מ-200 משתמשים בכל פעם, יותר מ-10,000 נמענים ביום, או יותר מ-30 הודעות בדקה.
- בעת הפעלת זרימת העבודה, הודעת הדואר האלקטרוני אינה נשלחת ואתה מבחין בהתנהגות הבאה:
    - עבור זרימת עבודה באמצעות סוג פלטפורמת SharePoint 2013, אתה גולש לדף ' **מצב זרימת עבודה** '. בדף ' מצב זרימת עבודה ', **המצב הפנימי** מוגדר **כהתחלתי**ובבלון המידע מציג **אפשרות לשלוח לנמען**.

כדי לעקוף בעיה זו, הגדר את זרימת העבודה שלך לשליחת הודעות דואר אלקטרוני מבלי לחרוג [ממגבלות השולח המקוון של Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). לדוגמה, השתמש בהשהיה בזרימת העבודה, שלח את הדואר האלקטרוני לקבוצת Office 365, קבוצת תפוצה או קבוצת אבטחה זמינה בדואר, או שלח את ההודעה לפחות מ-200 נמענים בכל פעם.


לקבלת מידע נוסף, עיין [במאמר](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)הבא.

## <a name="related-topics"></a>נושאים קשורים
- [צור זרימה](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint וזרימה](https://flow.microsoft.com/blog/sharepoint-and-flow/) 