---
title: לזהות אירועים ההודעה מחק יומני ביקורת
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909281"
---
# <a name="audit-logs-for-deleted-email-messages"></a>יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו

החל ב- 2019 בינואר, הוא הפעלת Microsoft ביקורת תיבות דואר רישום כברירת מחדל. אחרת, כדי לסקור את אירועי הודעת מחיקה עבור משתמש מסוים, עליך לאפשר באופן ידני את פעולות מחיקה לביקורת. אם תיבת הדואר ביקורת רישום כבר זמין עבור הארגון שלך או עבור משתמש מסוים, בצע את השלבים הבאים.

1. היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/)

2. לחץ על **חיפוש ויצירת החקירה** ובחר באפשרות **החיפוש יומן ביקורת**.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** . ציין את שם המשתמש עבור המשתמש שברצונך לבדוק (המשתמש על הפריטים שנמחקו). בשדה ' **פעילויות** ', בחר **הודעות שנמחקו מהתיקיה פריטים שנמחקו** והודעות **Moved לתיקיה פריטים שנמחקו**.

4. לחץ על **חיפוש**.

בתוצאות, בחר את רשומת הביקורת. תפריט נשלף של פרטים, לחץ על **מידע נוסף**. מידע נוסף אודות הפריט שנמחק (לדוגמה, את שורת הנושא ואת המיקום של הפריט בעת שהוא נמחק) מוצג בשדה **AffectedItems** . המאפיין **ClientInfoString** יציג אם המחיקה אירעה ב- Outlook, Outlook באינטרנט (שכונתה בעבר Outlook Web App), או כל התקן אחר.

לקבלת מידע נוסף, ראה [קביעת שהגדיר העברה עבור תיבת דואר אלקטרוני](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**הערה**: אין אפשרות לאחזר פריטים שנמחקו באמצעות התכונה ביומן הביקורת. כדי לאחזר הודעות שנמחקו ב- Outlook באינטרנט, ראה [שחזור פריטים ב- Outlook Web App שנמחקו](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
