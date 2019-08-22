---
title: חריגה ממגבלת דואר אלקטרוני יומי. זרימת עבודה מושעית.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514455"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>חריגה ממגבלת דואר אלקטרוני יומי. זרימת עבודה מושעית.

שגיאה זו עשויה להתקבל בתרחישים הבאים:

- יש לך זרימת עבודה ב- SharePoint במצב מקוון שבו הוא משתמש SharePoint 2010 או סוג פלטפורמה זרימת עבודה של SharePoint 2013.
- זרימת העבודה נקבעה כדי לשלוח הודעת דואר אלקטרוני מותאמות אישית משתמשים יותר מ- 200 בכל פעם, למעלה מ- 10,000 נמענים בכל יום או יותר מ- 30 הודעות לדקה.
- כאשר אתה מפעיל את זרימת העבודה, ההודעה לא תישלח ולאחר תבחין בהתנהגות הבאה:
    - עבור זרימת עבודה באמצעות סוג פלטפורמת SharePoint 2013, דפדף אל דף **מצב זרימת העבודה** . בדף ' מצב זרימת עבודה ', **מצב פנימי** מוגדר **הופעל**, ומציג בלון המידע **אין אפשרות לשלוח לנמען**.

כדי לעקוף בעיה זו, קביעת התצורה של זרימת העבודה שלך כדי לשלוח הודעות דואר אלקטרוני מבלי לחרוג [ממגבלות השולח Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). לדוגמה, השתמש השהיה בזרימת העבודה, הדואר האלקטרוני לקבוצה Office 365, קבוצת תפוצה או קבוצת אבטחה דואר זמין או לשלוח את ההודעה לנמענים פחות מ- 200 בכל פעם.


לקבלת מידע נוסף, עיין [במאמר](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)הבא.

## <a name="related-topics"></a>נושאים קשורים
- [צור זרימה](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint וזרימה](https://flow.microsoft.com/blog/sharepoint-and-flow/) 