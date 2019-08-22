---
title: התיקיה RecoverableItems 1336 הוא מלא
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 8a5859ba29d847606e8b44d169c3cd6a26364744
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36509739"
---
# <a name="the-recoverable-items-folder-is-full"></a>התיקיה פריטים ניתנים לשחזור הוא מלא

עבור תיבות דואר Exchange Online ב- Office 365, מגבלת האחסון המוגדר כברירת מחדל עבור התיקיה פריטים ניתנים לשחזור הוא 30 ג'יגה-בתים. מגבלת האחסון עבור התיקיה פריטים ניתנים לשחזור באופן אוטומטי יגדל עד 100 ג'יגה-בתים אם תיבת הדואר ממוקם על החזק תביעה משפטית, גילוי אלקטרוני בהמתנה, או מוקצה למדיניות השמירה של Office 365.

כאשר התיקיה פריטים ניתנים לשחזור הגיע למגבלת האחסון, פונקציונליות תיבת הדואר מושפע בדרכים הבאות:

- למשתמש אין אפשרות למחוק פריטים מתיבת הדואר.

- מנוהל מסייע התיקיות אין אפשרות למחוק פריטים לפי תגית שמירה או הגדרות תיקיות מנוהלות.

- עבור תיבות דואר זמין שחזור פריט יחיד או ממוקמים בהמתנה, תהליך הגנת עמוד עותק בעת כתיבה לא ניתן לשמור על גירסאות של פריטים שנערכו על-ידי המשתמש.

- עבור תיבות דואר שיש להם תיבת דואר ביקורת הרישום זמין, ניתן לשמור ללא ערכי יומן ביקורת של תיבת דואר בתיקיית המשנה ביקורות בתיקיה פריטים ניתנים לשחזור.

עבור תיבות דואר שאינן בהמתנה, מנהלים יכולים להשתמש `Search-Mailbox -SearchDumpsterOnly -DeleteContent` הפקודה ב- Exchange Online PowerShell למחיקת פריטים בתיקיה פריטים ניתנים לשחזור. כדי לקבל מידע נוסף עיין בנושאים הבאים:

- [חיפוש ומחיקה של הודעות](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [חיפוש-תיבת דואר](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

עבור תיבות דואר הנמצאות בהמתנה, המנהלים צריך להסיר את החסימה לפני שהם יכולים פריטים שנמחקו מהתיקיה פריטים ניתנים לשחזור. לקבלת מידע נוסף, ראה [מחיקת פריטים בפריטים ניתן לשחזר תיקיה של תיבות דואר מבוססות ענן על החזק](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

כדי לסייע למנוע את התיקיה פריטים ניתנים לשחזור והופך מלאה, מנהלים באפשרותך להגדיל את המגבלה אחסון של פריטים ניתנים לשחזור תיקיה עבור תיבות דואר על החזק ולהגדיר את מדיניות השמירה תיבת הדואר המעביר פריטים מהתיקיה פריטים ניתנים לשחזור לארכיון של המשתמש תיבת הדואר. ראה [להגדיל פריטים ניתנים לשחזור החזק מיכסה עבור תיבות דואר ב-](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
