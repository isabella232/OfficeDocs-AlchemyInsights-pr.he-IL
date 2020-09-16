---
title: התוספת teams עבור Mac
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670329"
---
# <a name="teams-add-in-for-mac"></a>התוספת teams עבור Mac

כדי לפתור בעיות של תוספת של צוותים חסרים עבור משתמשי מערכת ההפעלה של Mac, בצע את הפעולות הבאות:

**שלב 1:** אם יש לך Exchange היברידי מקומי (2016 CU3 או מאוחר יותר נדרש), השתמש Test-HMA.ps1 בכלי כדי לאשר שאימות מודרני משולב מוגדר כהלכה. לקבלת מידע נוסף, ראה [אימות הגדרת אימות מודרנית היברידית עבור Outlook עבור iOS ו-Android](https://aka.ms/AA980zq).  

**הערה** השתמש בתבנית כתובת UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)), לא domain\username. עשה זאת גם עבור משתמשים בעלי תיבות דואר של Exchange Online.

**שלב 2:** העבר את המשתמש **Tools**  >  **לחשבונות**כלים... ב-Outlook עבור Mac, וחפש את החשבון ובחר אותו. אשר את שם המשתמש המופיע בתבנית UPN (לדוגמה, [username@contoso.com](mailto:username@contoso.com)).

**שלב 3:** אשר שהמשתמש הוא משתמש מורשה של Microsoft Teams. על המשתמש להשתמש במנוי Office 365 for Mac, בגירסה 16.24 ואילך.