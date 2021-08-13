---
title: העברת הודעות דואר אלקטרוני לתיבת הדואר של ארכיון
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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974958"
---
# <a name="move-email-to-the-archive-mailbox"></a>העברת דואר אלקטרוני לתיבת הדואר של הארכיון

אם ברצונך שנריץ בדיקות אוטומטיות עבור ההגדרות שהוזכרו להלן, בחר את לחצן הקודם <- בחלק העליון של דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שיש לו בעיות בהזזת דואר אלקטרוני לתיבת הדואר שלו בארכיון.

1. ודא שתיבת **דואר של** ארכיון הופעלה. אם לא, השתמש בשלבים המפורטים [במאמר זה כדי להפוך את](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) תיבת הדואר של הארכיון לזמינה.

2. כדי לאחסן הודעות בארכיון באופן אוטומטי  בתיבת הדואר של הארכיון, יש להגדיר תגית שמירה עם הפעולה העבר לארכיון לחלה אוטומטית על תגית תיבת הדואר **כולה (ברירת המחדל).** השתמש בשלבים כאן כדי ליצור את התגית: תגית [ברירת מחדל בארכיון](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. לאחר מכן, הוסף את **תגית** הארכיון למדיניות השמירה שלך. במרכז הניהול Exchange, בחר **מדיניות** שמירה > את התגית העבר **לארכיון** למדיניות > **שמור**.

4. כעת [הקצה את מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) לתיבת הדואר של המשתמש הספציפי. אותה מדיניות תחול הן על תיבת הדואר **הראשית ועל** תיבת הדואר **של ארכיון.**

ייתכן שיהיה צורך לכפות על מסייע התיקיות המנוהלים (MFA) לפעול ולהחיל את ההגדרות החדשות על תיבת הדואר של המשתמש. הפעל את הפקודה הבאה בזמן [שאתה מחובר ל- EXO PowerShell כדי](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) להפעיל את מסייע התיקיות המנוהלים עבור תיבת דואר ספציפית:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

לקבלת מידע נוסף אודות הגדרת מדיניות ארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה עבור תיבות דואר.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  