---
title: העברת הודעות דואר אלקטרוני לתיבת הדואר של הארכיון
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799781"
---
# <a name="move-email-to-the-archive-mailbox"></a>העברת דואר אלקטרוני לתיבת הדואר של הארכיון

אם ברצונך לבצע בדיקות אוטומטיות עבור ההגדרות המוזכרות להלן, בחר את לחצן ' הקודם ' < '-בחלק העליון של דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שנתקל בבעיות בהעברת דואר אלקטרוני לתיבת הדואר של הארכיון.

1. ודא **שתיבת דואר של ארכיון** הופעלה. אם לא, השתמש בשלבים המפורטים [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) כדי להפוך את תיבת הדואר של הארכיון לזמינה.

2. כדי לאחסן בארכיון הודעות באופן אוטומטי בתיבת הדואר של הארכיון, יש להגדיר תגית שמירה עם הפעולה ' **העבר לארכיון** ' כדי **להחיל אותה באופן אוטומטי על התגית תיבת דואר מלאה (ברירת מחדל)**. השתמש בשלבים הבאים כדי ליצור את התגית: [תג ברירת המחדל של הארכיון](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. לאחר מכן, הוסף את תג **הארכיון** למדיניות השמירה. במרכז הניהול של Exchange, בחר **מדיניות שמירה** > הוסף את **התגית ' העבר לארכיון** ' למדיניות > **Save**.

4. כעת [הקצה את מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) לתיבת הדואר של המשתמש הספציפי. מדיניות זו תחול על תיבת הדואר **הראשית** והן עבור תיבת הדואר של **הארכיון** .

ייתכן שיהיה צורך לאלץ את מסייע התיקיות המנוהלות (מנהל המשרד) לפעול ולהחיל את ההגדרות החדשות על תיבת הדואר של המשתמש. הפעל את הפקודה הבאה כאשר אתה [מחובר ל-קליפת PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר ספציפית:
  
Start-ManagedFolderAssistant-זהות <name of the mailbox>

לקבלת מידע נוסף אודות הגדרת מדיניות ארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה עבור תיבות דואר](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  