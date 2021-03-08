---
title: חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524283"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך

בצע שלבים אלה:

1. אם אינך מנהל מערכת כללי, כדי לחפש הודעות יש להוסיף את החשבון שלך **לקבוצת התפקידים ' מנהל גילוי אלקטרוני** ' או **לתפקיד ניהול חיפוש התאימות**. כדי למחוק הודעות, יהיה עליך להצטרף **לקבוצת התפקידים ' ניהול ארגון** ' או **לתפקיד הניהול ' חיפוש וניקוי**'. הרשאות לתפקידים אלה מוקצות [במרכז התאימות של אבטחה &.](https://protection.office.com)
2. [צור חיפוש תוכן](https://docs.microsoft.com/office365/securitycompliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.
3. [התחבר אל מרכז התאימות של אבטחה & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). אם אתה משתמש במרכז המדינה, ראה הוראות אלה: [התחברות לאבטחה & מרכז התאימות של PowerShell באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. מחק את ההודעה: הפעיל את ה `New-ComplianceSearchAction` -cmdlet כדי למחוק את ההודעה. הודעות שנמחקו מועברות לתיקיה ' פריטים הניתנים לשחזור ' של משתמש. לקבלת פקודה לדוגמה, ראה [שלב 3: מחיקת ההודעה.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
