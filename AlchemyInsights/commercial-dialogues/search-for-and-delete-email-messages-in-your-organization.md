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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948884"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך

בצע שלבים אלה:

1. אם אינך מנהל מערכת כללי, כדי לחפש הודעות יש להוסיף את החשבון שלך לקבוצת התפקידים **מנהל** גילוי אלקטרוני או לתפקיד **ניהול חיפוש תאימות**. כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת **התפקידים 'ניהול ארגוני'** או לתפקיד ניהול **חיפוש ומחיקה.** הרשאות לתפקידים אלה מוקצות במרכז האבטחה [& תאימות.](https://protection.office.com)
2. [צור חיפוש תוכן כדי](https://docs.microsoft.com/office365/securitycompliance/content-search) למצוא את ההודעה למחיקה.
3. [התחברות ל- PowerShell & האבטחה של מרכז התאימות.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) אם אתה משתמש ב- MFA, עיין בהוראות אלה: [התחברות אל מרכז & תאימות של PowerShell באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. מחק את ההודעה: הפעל את `New-ComplianceSearchAction` ה- cmdlet כדי למחוק את ההודעה. הודעות שנמחקו מועברות לתיקיה 'פריטים הניתנים לשחזור' של משתמש. לקבלת פקודה לדוגמה, ראה [שלב 3: מחיקת ההודעה.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
