---
title: Exchange PowerShell והוצאה משימוש של אימות בסיסי
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813473"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell והוצאה משימוש של אימות בסיסי

לקבלת המידע העדכני ביותר על כיצד להתחבר ל- Exchange Online PowerShell ללא שימוש באימות בסיסי, [עבור לכאן](https://aka.ms/exops-docs). מודול PowerShell V2 אינו משתמש באימות בסיסי.

שים לב שאימות בסיסי עדיין צריך להיות זמין במחשב הלקוח.
המודול החדש של PowerShell V2 משתמש באימות מודרני כדי ליצור חיבור להפעלה של כל רכיבי V2 Cmdlet מבוססי REST. בנוסף לרכיבי V2 cmdlet, הוא גם מאפשר לך לגשת לרכיבים קודמים של Cmdlet של PowerShell מרוחק (RPS), שדורשים הפעלה של PowerShell מרוחק. יצירת הפעלת RPS במחשב Windows דורשת ש-WinRM BasicAuth יהיה זמין במחשב הלקוח למרות שהמודול משתמש במנגנון אימות מודרני כדי לאמת את השירות. צינור האימות הבסיסי של WinRM משמש להובלת אסימוני אימות מודרניים. אם האימות הבסיסי של WinRM אינו זמין במחשב הלקוח, רכיבי ה-V2 cmdlet החדשים ימשיכו לפעול (אך רכיבי ה- cmdlet הקודמים של RPS לא ימשיכו לפעול).
