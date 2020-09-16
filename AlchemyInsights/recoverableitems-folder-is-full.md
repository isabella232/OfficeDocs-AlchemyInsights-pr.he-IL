---
title: התיקיה RecoverableItems של 1336 מלאה
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741268"
---
# <a name="the-recoverable-items-folder-is-full"></a>התיקיה ' פריטים הניתנים לשחזור ' מלאה

עבור תיבות דואר של Exchange Online, מגבלת האחסון המוגדרת כברירת מחדל עבור התיקיה ' פריטים הניתנים לשחזור ' היא 30 GB. מגבלת האחסון עבור התיקיה ' פריטים הניתנים לשחזור ' מוגברת באופן אוטומטי ל-100 GB אם תיבת הדואר ממוקמת בחסימה לצורך תביעה משפטית, גילוי אלקטרוני Hold או מוקצית למדיניות שמירה.

כאשר התיקיה ' פריטים הניתנים לשחזור ' מגיעה למגבלת האחסון, פונקציונליות תיבת הדואר מושפעת בדרכים הבאות:

- למשתמש אין אפשרות למחוק פריטים מתיבת הדואר.

- לעוזר התיקיה המנוהלת אין אפשרות למחוק פריטים בהתבסס על תגית שמירה או הגדרות תיקיה מנוהלת.

- עבור תיבות דואר שבהן שחזור פריט בודד זמין או ממוקמות בהמתנה, תהליך ההגנה על דף ההעתקה-כתיבה אינו יכול לשמור גירסאות של פריטים שנערכו על-ידי המשתמש.

- עבור תיבות דואר הכוללות רישום ביקורת של תיבות דואר זמין, לא ניתן לשמור ערכי יומן ביקורת של תיבות דואר בתיקיית המשנה ' ביקורות ' בתיקיה ' פריטים הניתנים לשחזור '.

עבור תיבות דואר שאינן בהמתנה, מנהלי מערכת יכולים להשתמש `Search-Mailbox -SearchDumpsterOnly -DeleteContent` בפקודה ב-Exchange Online PowerShell כדי למחוק פריטים בתיקיה ' פריטים הניתנים לשחזור '. כדי לקבל מידע נוסף עיין בנושאים הבאים:

- [חיפוש ומחיקה של הודעות](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [חיפוש-תיבת דואר](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

עבור תיבות דואר הנמצאות בהמתנה, מנהלי מערכת חייבים להסיר את החסימה לפני שיוכלו למחוק פריטים מהתיקיה ' פריטים הניתנים לשחזור '. לקבלת מידע נוסף, ראה [מחיקת פריטים בתיקיה ' פריטים הניתנים לשחזור ' של תיבות דואר מבוססות ענן בהמתנה](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

כדי לסייע במניעת השלמות של התיקיה ' פריטים הניתנים לשחזור ', מנהלי מערכת יכולים להגדיל את מגבלת האחסון של התיקיה ' פריטים הניתנים לשחזור ' עבור תיבות דואר בהמתנה ולהגדיר מדיניות שמירה של תיבת דואר שמעבירה פריטים מהתיקיה ' פריטים הניתנים לשחזור ' לתיבת הדואר של המשתמש ראה [הגדלת מיכסת הפריטים הניתנים לשחזור עבור תיבות דואר בהמתנה](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
