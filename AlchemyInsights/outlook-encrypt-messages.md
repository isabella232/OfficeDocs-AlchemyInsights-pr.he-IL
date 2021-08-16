---
title: S/MIME Outlook באינטרנט
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010725"
---
# <a name="encrypt-email-messages-in-outlook"></a>הצפן הודעות דואר אלקטרוני Outlook

Microsoft 365 הצפנת הודעות מבוססת על Microsoft Azure Rights Management (Azure RMS), שהוא חלק מ- Azure Information Protection. אם המנוי שלך כולל את Azure Rights Management או Azure Information Protection, אין צורך לבצע פעולות כדי להפעיל או להפעיל באופן ידני **את** שירות ניהול הזכויות.

בהתבסס על משוב מלקוחות, לא נאפשר עוד לכללי Exchange זרימת דואר להצפין באופן אוטומטי דואר אלקטרוני יוצא המכיל סוג מסוים של מידע רגיש דייר כברירת מחדל. במקום זאת, אנו מספקים הוראות מפורטות כיצד תוכלו לעשות זאת בעצמכם. לקבלת פרטים נוספים אודות יצירת כלל תעבורה להצפנת מידע רגיש, [עיין במאמר זה](https://aka.ms/OmeEtr).

- אם אתה משתמש Outlook באינטרנט (לשעבר **OWA):** בעת חיבור הודעת דואר אלקטרוני, פשוט לחץ על **הגן ב-** OWA. פעולה זו תחיל הרשאת "אל תעביר". לחץ **על שנה הרשאה** ובחר **הצפן** כדי להצפין את ההודעה בלבד.

- אם אתה **משתמש בלקוח Outlook**: כדי לשלוח הודעה מוצפנת מ- Outlook 2013 או מ- 2016, או Outlook 2016 עבור Mac, בחר אפשרויות הרשאות ולאחר מכן בחר באפשרות  >  ההגנה הדרושה.

- כדי **להצפין באופן אוטומטי** את כל הדואר האלקטרוני שנשלח לנמענים מסוימים או לארגונים של שותפים חיצוניים, עליך ליצור כלל תעבורה של זרימת דואר במרכז Exchange הניהול. הוראות מפורטות מסופקות [במאמר תמיכה זה](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

