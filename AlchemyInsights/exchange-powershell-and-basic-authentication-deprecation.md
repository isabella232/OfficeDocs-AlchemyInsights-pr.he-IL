---
title: Exchange PowerShell והוצאה משימוש של אימות בסיסי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015690"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell והוצאה משימוש של אימות בסיסי

לקבלת המידע העדכני ביותר על כיצד להתחבר ל- Exchange Online PowerShell ללא שימוש באימות בסיסי, [עבור לכאן](https://aka.ms/psbasicauth).

שים לב שאימות בסיסי עדיין צריך להיות זמין במחשב הלקוח.
המודול החדש של PowerShell V2 משתמש באימות מודרני כדי ליצור חיבור להפעלה של כל רכיבי V2 Cmdlet מבוססי REST. בנוסף לרכיבי V2 cmdlet, הוא גם מאפשר לך לגשת לרכיבים קודמים של Cmdlet של PowerShell מרוחק (RPS), שדורשים הפעלה של PowerShell מרוחק. יצירת הפעלת RPS במחשב Windows דורשת ש-WinRM BasicAuth יהיה זמין במחשב הלקוח למרות שהמודול משתמש במנגנון אימות מודרני כדי לאמת את השירות. צינור האימות הבסיסי של WinRM משמש להובלת אסימוני אימות מודרניים. אם האימות הבסיסי של WinRM אינו זמין במחשב הלקוח, רכיבי ה-V2 cmdlet החדשים ימשיכו לפעול (אך רכיבי ה- cmdlet הקודמים של RPS לא ימשיכו לפעול).
