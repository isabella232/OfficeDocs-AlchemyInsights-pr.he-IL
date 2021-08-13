---
title: תיקיית RecoverableItems 1336 מלאה
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061757"
---
# <a name="the-recoverable-items-folder-is-full"></a>התיקיה 'פריטים הניתנים לשחזור' מלאה

עבור Exchange Online, מגבלת האחסון המוגדרת כברירת מחדל עבור התיקיה 'פריטים הניתנים לשחזור' היא 30 GB. מגבלת האחסון עבור התיקיה 'פריטים הניתנים לשחזור' מוגדלת באופן אוטומטי ל- 100 GB אם תיבת הדואר ממוקמת בחסימה לתביעה משפטית, בחסימה של גילוי אלקטרוני או מוקצית למדיניות שמירה.

כאשר התיקיה 'פריטים הניתנים לשחזור' מגיעה למגבלת האחסון, פונקציונליות תיבת הדואר מושפעת בדרכים הבאות:

- למשתמש אין אפשרות למחוק פריטים מתיבת הדואר.

- למסייע התיקיות המנוהלים אין אפשרות למחוק פריטים בהתבסס על תגית שמירה או הגדרות תיקיה מנוהלת.

- עבור תיבות דואר שהאפשרות שחזור פריט יחיד זמינה או ממוקמות בהמתנה, תהליך ההגנה על הדף 'העתקה בכתיבה' אינו יכול לשמור גירסאות של פריטים שנערך על-ידי המשתמש.

- עבור תיבות דואר שרישום ביקורת של תיבת דואר זמין, לא ניתן לשמור ערכי יומן ביקורת של תיבת דואר בתיקיית המשנה 'ביקורות' בתיקיה 'פריטים הניתנים לשחזור'.

עבור תיבות דואר שלא נמצאות בהמתנה, מנהלי מערכת יכולים להשתמש בפקודה `Search-Mailbox -SearchDumpsterOnly -DeleteContent` ב- Exchange Online PowerShell כדי למחוק פריטים בתיקיה 'פריטים הניתנים לשחזור'. כדי לקבל מידע נוסף עיין בנושאים הבאים:

- [חיפוש ומחיקה של הודעות](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

עבור תיבות דואר בהמתנה, מנהלי מערכת צריכים להסיר את ההמתנה לפני שהם יכולים למחוק פריטים מהתיקיה 'פריטים הניתנים לשחזור'. לקבלת מידע נוסף, ראה [מחיקת פריטים בתיקיה 'פריטים הניתנים לשחזור' של תיבות דואר המבוססות על ענן צמתים בהמתנה](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

כדי לסייע במניעת ההגדלה של התיקיה 'פריטים הניתנים לשחזור', מנהלי מערכת יכולים להגדיל את מגבלת האחסון של התיקיה 'פריטים הניתנים לשחזור' עבור תיבות דואר בהמתנה ולהגדיר מדיניות שמירה של תיבות דואר המ מעבירה פריטים מהתיקיה 'פריטים הניתנים לשחזור' לתיבת הדואר של הארכיון של המשתמש. ראה [הגדלת מיכסת הפריטים הניתנים לשחזור עבור תיבות דואר בהמתנה](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
