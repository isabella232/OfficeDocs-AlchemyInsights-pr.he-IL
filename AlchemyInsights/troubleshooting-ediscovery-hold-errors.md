---
title: פתרון בעיות ב- ediscovery כולל שגיאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676150"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>פתרון בעיות ב- ediscovery כולל שגיאות

נתקל בבעיות עם החזקות גילוי אלקטרוני? להלן כמה שיטות עבודה מומלצות שיש לשקול:

- בדוק את מצב ההפצה של החזקה.  אם המצב פעיל **(ממתין)** או **כבוי (ממתין),** המתן להשלמת התפלגות החזקה.
- מזג עדכונים של גילוי אלקטרוני לאחסון עדכונים בבקשה בצובר אחת במקום לעדכן את המדיניות שוב ושוב עבור כל טרנזקציה.
- הפעל Set-CaseHoldPolicy <policyname> -retryDistribution in the Security and Compliance Center Powershell. לקבלת פרטים, [ראה התחברות אל מרכז & תאימות של PowerShell](/powershell/exchange/connect-to-scc-powershell).

לקבלת שלבים כדי לבדוק הגדרות אלה ושיטות עבודה מומלצות נוספות להקלה ופתרון של גילוי אלקטרוני תפתור בעיות, ראה פתרון שגיאות בהמתנה [של גילוי אלקטרוני.](/microsoft-365/compliance/hold-distribution-errors)
לקבלת מידע אודות פתרון בעיות נפוצות אחרות של גילוי אלקטרוני, ראה [חקירה, פתרון בעיות](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)נפוצות של גילוי אלקטרוני ופתרון בעיות נפוצות ב גילוי אלקטרוני.
