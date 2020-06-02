---
title: זיהוי אירועי הודעות מחיקה ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508989"
---
# <a name="audit-logs-for-deleted-email-messages"></a>יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו

החל מינואר 2019, Microsoft מופעלת כברירת מחדל ברישום ביקורת תיבת דואר. אחרת, כדי לסקור אירועי הודעה עבור משתמש מסוים, עליך להפוך באופן ידני את פעולות המחיקה לביקורת. אם רישום ביקורת תיבת דואר זמין כבר עבור הארגון שלך או עבור המשתמש הספציפי, בצע את השלבים שלהלן.

1. היכנס ל- [Microsoft 365 האבטחה _ Ampp_e מרכז התאימות](https://protection.office.com/)

2. לחץ על **חיפוש וחקירה** ובחר **חיפוש יומן רישום ביקורת**.

3. בחר את טווח התאריכים **בתאריך ההתחלה** ושדות **הסיום** . ציין שם משתמש עבור המשתמש שברצונך לחקור (המשתמש שמחק את הפריטים). בשדה ' **פעילויות** ', בחר **הודעות שנמחקו מהתיקיה ' פריטים שנמחקו** ' והעברת **הודעות לפריטים שנמחקו**.

4. לחץ על **חיפוש**.

בתוצאות, בחר ברשומת ביקורת. בתפריט הפרטי, לחץ על **מידע נוסף**. מידע נוסף אודות הפריט שנמחק (לדוגמה, שורת הנושא ומיקום הפריט בעת המחיקה) מוצג בשדה ' **הקצאת** המים '. המאפיין **מחרוזת לקוחוה** יציג אם המחיקה התרחשה ב-Outlook, outlook באינטרנט (הידוע בעבר כ-Outlook web App), או כל התקן אחר.

לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**הערה**: לא ניתן לאחזר פריטים שנמחקו באמצעות תכונת יומן הביקורת. כדי לאחזר הודעות שנמחקו ב-Outlook באינטרנט, ראה [שחזור פריטים שנמחקו ב-Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
