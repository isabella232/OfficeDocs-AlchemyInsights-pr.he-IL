---
title: Teams תוספת עבור Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940676"
---
# <a name="teams-add-in-for-mac"></a>Teams תוספת עבור Mac

כדי לפתור בעיות של Teams עבור משתמשי מערכת ההפעלה Mac, בצע את הפעולות הבאות:

**שלב 1:** אם יש לך Exchange היברידי מקומי (2016 CU3 ואילך נדרש), השתמש בכלי Test-HMA.ps1 כדי לוודא שתצורת האימות המודרנית ההיברידית נקבעה כראוי. לקבלת מידע נוסף, ראה [אימות הגדרת אימות מודרני היברידי עבור Outlook עבור iOS ו- Android](https://aka.ms/TestHMAEAS).  

**הערה** השתמש בתבנית כתובת UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)), ולא domain\username. בצע פעולה זו גם עבור משתמשים בעלי Exchange Online דואר.

**שלב 2:** האם המשתמש י לעבור אל **'חשבונות**  >  **כלים'**... ב- Outlook עבור Mac, ומצא ובחר את החשבון. אשר את שם המשתמש המפורט בתבנית UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)).

**שלב 3:** אשר שהמשתמש הוא משתמש מורשה Microsoft Teams משתמש. המשתמש חייב להשתמש במנוי Office 365 עבור Mac, במוצר גירסה 16.24 ואילך.