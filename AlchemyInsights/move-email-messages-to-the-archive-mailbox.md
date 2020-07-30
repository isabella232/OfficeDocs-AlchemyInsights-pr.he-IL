---
title: העברת הודעות דואר אלקטרוני לתיבת הדואר ' ארכיון '
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522772"
---
# <a name="move-email-to-the-archive-mailbox"></a>העברת דואר אלקטרוני לתיבת הדואר של הארכיון

אם ברצונך שנריץ בדיקות אוטומטיות עבור ההגדרות שהוזכרו להלן, בחר את לחצן החזרה _ Lt_--בראש דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שיש לו בעיות בהעברת הדואר האלקטרוני לתיבת הדואר שלהם בארכיון.

1. ודא **שתיבת דואר של ארכיון** הופעלה. אם לא, השתמש בשלבים [שבמאמר זה](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) כדי להפוך את תיבת הדואר של הארכיון לזמינה.

2. כדי לאחסן בארכיון הודעות באופן אוטומטי לתיבת הדואר של הארכיון, יש להגדיר תג שמירה עם **העברת לפעולה בארכיון** כך **שיוחל באופן אוטומטי על תג תיבת הדואר המלא (ברירת המחדל)**. השתמש בשלבים כאן כדי ליצור את התג: [התגית ' ברירת מחדל של ארכיון](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)'.

3. לאחר מכן, הוסף את תג **הארכיון** למדיניות השמירה. במרכז הניהול של Exchange, בחר באפשרות **מדיניות שמירה** _ gtie הוסף את **המעבר לתגית ארכיון** למדיניות _ **שמירה**.

4. כעת [הקצה את מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) לתיבת הדואר של המשתמש הספציפי. אותה מדיניות תוחל הן על תיבת הדואר **הראשית** והן של **הארכיון** .

ייתכן שיהיה צורך לכפות על מסייע התיקיות המנוהלות (משרד המשנה) להפעיל ולהחיל את ההגדרות החדשות על תיבת הדואר של המשתמש. הפעל את הפקודה הבאה בעת [ההתחברות ל-EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר ספציפית:
  
מסייע מניהול התחל-זהות<name of the mailbox>

לקבלת מידע נוסף אודות הגדרת מדיניות ארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה עבור תיבות דואר](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  