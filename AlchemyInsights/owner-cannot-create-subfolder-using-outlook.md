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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063125"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>הבעלים אינו יכול ליצור תיקיית משנה באמצעות Outlook

**קיימת בעיה מתמשכת עם בעלי תיקיות ציבוריות שיוצרים תיקיות משנה באמצעות Outlook. הבעיה תתוקן בקרוב.**

בינתיים, השתמש באחת מהדרכים הבאות לעקיפת הבעיה:

1. השתמש Outlook עבור MAC כדי ליצור את תיקיית המשנה כאשר הבעיה משפיעה רק Outlook עבור חלונות שולחניים (כל הגירסאות)
2. יש למנהל מערכת ליצור את תיקיית המשנה באמצעות EXO Shell או EAC
3. שינוי DefaultציבוריFolderMailbox/EffectivePublicFolderMailbox על המשתמש לתיבת דואר אחרת מאשר תיבת הדואר של התוכן עבור התיקיה שגרמה לבעיה  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. המתן שעה, הפעל מחדש את לקוח Outlook