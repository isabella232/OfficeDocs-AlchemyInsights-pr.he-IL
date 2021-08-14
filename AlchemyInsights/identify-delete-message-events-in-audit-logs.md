---
title: זיהוי אירועי מחיקת הודעות ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868419"
---
# <a name="audit-logs-for-deleted-email-messages"></a>יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו

החל מינואר 2019, Microsoft מפעילה רישום ביקורת של תיבת דואר כברירת מחדל. אחרת, כדי לסקור אירועי מחיקה של הודעות עבור משתמש ספציפי, עליך להפוך את פעולות המחיקה לזמינות באופן ידני עבור ביקורת. אם רישום ביקורת תיבת דואר כבר זמין עבור הארגון שלך או עבור המשתמש הספציפי, בצע את השלבים הבאים.

1. היכנס למרכז [Microsoft 365 התאימות](https://protection.office.com/)

2. לחץ **על חיפוש וחקירה** ובחר **חיפוש ביומן ביקורת**.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך** סיום. ציין שם משתמש עבור המשתמש שברצונך לחקור (המשתמש שמחקת את הפריטים). בשדה **פעילויות,** בחר הודעות שנמחקו **מהתיקיה פריטים** שנמחקו והודעות **הועברו לתיקיה פריטים שנמחקו**.

4. לחץ **על חיפוש**.

בתוצאות, בחר רשומת ביקורת. בפרטים נשלף, לחץ **על מידע נוסף**. מידע נוסף אודות הפריט שנמחק (לדוגמה, שורת הנושא ומיקום הפריט בעת מחיקתו) מוצגים בשדה **AffectedItems.** המאפיין **ClientInfoString** יופיע אם המחיקה התרחשה ב- Outlook, Outlook באינטרנט (נקרא בעבר Outlook Web App) או כל מכשיר אחר.

לקבלת מידע נוסף, [ראה קביעת מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**הערה:** לא ניתן לאחזר פריטים שנמחקו באמצעות תכונת יומן הביקורת. כדי לאחזר הודעות שנמחקו ב- Outlook באינטרנט, ראה [שחזור פריטים שנמחקו ב- Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
