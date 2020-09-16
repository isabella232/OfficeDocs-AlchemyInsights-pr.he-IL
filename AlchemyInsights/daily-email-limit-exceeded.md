---
title: חריגה ממגבלת דואר אלקטרוני יומית. זרימת העבודה מושעית.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731564"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>חריגה ממגבלת דואר אלקטרוני יומית. זרימת העבודה מושעית.

שגיאה זו עשויה להתקבל בתרחישים הבאים:

- יש לך זרימת עבודה ב-SharePoint Online המשתמשת בסוג פלטפורמת זרימת העבודה של SharePoint 2010 או SharePoint 2013.
- זרימת העבודה מוגדרת לשליחת הודעת דואר אלקטרוני מותאמת אישית ליותר מ-200 משתמשים בכל פעם, יותר מ-10,000 נמענים לכל יום, או יותר מ-30 הודעות בדקה.
- כאשר תפעיל את זרימת העבודה, הודעת הדואר האלקטרוני לא תישלח ותשים לב לאופן הפעולה הבא:
    - עבור זרימת עבודה באמצעות סוג הפלטפורמה של SharePoint 2013, עליך לדפדף לדף ' **מצב זרימת עבודה** '. בדף ' מצב זרימת עבודה ', **המצב הפנימי** מוגדר **להתחיל**, ובלון המידע אינו מציג **אפשרות לשלוח לנמען**.

כדי לעקוף בעיה זו, קבע את התצורה של זרימת העבודה לשליחת הודעות דואר אלקטרוני מבלי לחרוג [ממגבלות השולח של Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). לדוגמה, השתמש בהשהיה בזרימת העבודה, שלח את הדואר האלקטרוני לקבוצה של Microsoft 365, קבוצת תפוצה או קבוצת אבטחה המותאמת לשימוש בדואר, או שלח את ההודעה לפחות מ-200 נמענים בכל פעם.


לקבלת מידע נוסף, עיין [במאמר](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)הבא.

## <a name="related-topics"></a>נושאים קשורים
- [יצירת זרימה](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ו-Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 