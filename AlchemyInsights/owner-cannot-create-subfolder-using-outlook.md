---
title: הבעלים אינו יכול ליצור תיקיית משנה באמצעות Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836136"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>הבעלים אינו יכול ליצור תיקיית משנה באמצעות Outlook

**קיימת בעיה מתמשכת עם בעלי תיקיות ציבוריות שיוצרים תיקיות משנה באמצעות Outlook. הבעיה תתוקן בקרוב.**

בינתיים, השתמש באחת מהדרכים הבאות לעקיפת הבעיה:

1. השתמש ב- Outlook עבור MAC כדי ליצור את תיקיית המשנה כאשר הבעיה משפיעה רק על Outlook עבור חלונות שולחן העבודה (כל הגירסאות)
2. יש למנהל מערכת ליצור את תיקיית המשנה באמצעות EXO Shell או EAC
3. שינוי DefaultציבוריFolderMailbox/EffectivePublicFolderMailbox על המשתמש לתיבת דואר אחרת מאשר תיבת הדואר של התוכן עבור התיקיה שגרמה לבעיה  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. המתן שעה, הפעל מחדש את לקוח Outlook