---
title: זיהוי מחיקת אירועי הודעות ביומני ביקורת
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696514"
---
# <a name="audit-logs-for-deleted-email-messages"></a>יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו

החל מ-2019 בינואר, Microsoft מפעיל רישום של ביקורת תיבת דואר כברירת מחדל. אחרת, כדי לסקור את מחיקת אירועי הודעות עבור משתמש ספציפי, עליך להפוך את פעולות המחיקה לזמינות באופן ידני עבור ביקורת. אם רישום ביקורת תיבת דואר כבר זמין עבור הארגון שלך או עבור המשתמש הספציפי, בצע את השלבים שלהלן.

1. היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/)

2. לחץ על **חיפוש וחקירה** ובחר **חיפוש ביומן הביקורת**.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך סיום** . ציין שם משתמש עבור המשתמש שברצונך לחקור (המשתמש שמחק את הפריטים). בשדה **פעילויות** , בחר **הודעות שנמחקו מתוך התיקיה ' פריטים שנמחקו** ' **והעברת הודעות לתיקיה ' פריטים שנמחקו**'.

4. לחץ על **חיפוש**.

בתוצאות, בחר רשומת ביקורת. בנשלף של הפרטים, לחץ על **מידע נוסף**. מידע נוסף אודות הפריט שנמחק (לדוגמה, שורת הנושא ומיקום הפריט כאשר הוא נמחק) מוצג בשדה **AffectedItems** . המאפיין **ClientInfoString** יציג אם המחיקה התרחשה ב-Outlook, outlook באינטרנט (שנקרא בעבר Outlook web App), או כל מכשיר אחר.

לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**הערה**: לא ניתן לאחזר פריטים שנמחקו באמצעות התכונה ' יומן ביקורת '. כדי לאחזר הודעות שנמחקו ב-Outlook באינטרנט, ראה [שחזור פריטים שנמחקו ב-Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
