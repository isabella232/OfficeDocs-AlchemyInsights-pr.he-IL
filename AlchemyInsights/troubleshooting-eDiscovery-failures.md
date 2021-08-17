---
title: 1490-פתרון בעיות-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105569"
---
# <a name="troubleshoot-content-search-errors"></a>פתרון בעיות של שגיאות חיפוש תוכן

האם אתה נתקל בבעיות בחיפוש תוכן או מקבל כשלים בעת ייצוא תוצאות חיפוש?

לדוגמה, האם אתה מקבל את הפעולות הבאות בעת הפעלת חיפושים?

- שגיאות CS008 או CS012

- שגיאות זמן קצוב/לא פנוי בשרת

- אירעה שגיאת יישום

לחלופין, בעת חיפוש או ייצוא של תוצאות ממספר גדול של תיבות דואר (מעל 100,000 תיבות דואר), האם אתה מקבל שגיאות ייצוא?

עבור סוגים אלה של שגיאות, נסה שוב לחפש את מיקומי התוכן שנכשלו. עיין  [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) לקבלת מידע נוסף.

אם אתה מייצא יותר מ- 100,000 תיבות דואר, יהיה עליך להשתמש ב- Powershell הבא כדי להוריד את תוצאות הייצוא: ייצוא תוצאות ביותר מתיבות דואר של  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
