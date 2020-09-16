---
title: לבעלים אין אפשרות ליצור תיקיית משנה באמצעות Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665719"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>לבעלים אין אפשרות ליצור תיקיית משנה באמצעות Outlook

**קיימת בעיה מתמשכת עם בעלי תיקיות ציבוריות שיוצרים תיקיות משנה באמצעות Outlook. הבעיה תתוקן בקרוב.**

בינתיים, השתמש באחת מהפתרונות הבאים:

1. שימוש ב-Outlook עבור MAC כדי ליצור את תיקיית המשנה כבעיה משפיעה רק על Outlook עבור windows desktop (כל הגירסאות)
2. ניהול מנהל המערכת צור את תיקיית המשנה באמצעות קליפת Shell או EAC
3. שינוי הDefaultPublicFolderMailbox/EffectivePublicFolderMailbox במשתמש לתיבת דואר אחרת מאשר תיבת הדואר של התוכן עבור הבעיה הגורמת לתיקיה  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. המתן לשעה, הפעל מחדש את לקוח outlook