---
title: פתרון בעיות בסנכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387878"
---
# <a name="troubleshoot-password-synchronization"></a>פתרון בעיות בסנכרון סיסמאות

כדי לפתור בעיות בסינכרון הסיסמאות, התחל בשימוש במשימה זו של פתרון בעיות של התחברות אד-משתמשים כדי לקבוע מדוע סיסמאות אינן מסינכרון. כדי להתחיל, עבור [לניהול סינכרון ישיר](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. פתח הפעלה חדשה של Windows PowerShell בשרת החיבור של תכלת AD שלך, ובחר באפשרות **הפעל כמנהל** .

2. הפעלה של מדיניות הגדרת המדיניות חתומה או הוגדרה מדיניות לא מוגבלת.

3. הפעל את אשף התקשרות תכלת.

4. עבור אל דף הפעילויות הנוספות _ gt_ **פתור**את הפעולות  >  **הבאות**.

5. בחר באפשרות ' **הפעלה** ' כדי לפתוח את תפריט פתרון בעיות PowerShell.

6. בחר **בפתרון בעיות בסינכרון סיסמאות**.

    הבעיה היא בדרך כלל שסיסמה אינה מסונכרנת עבור חשבון משתמש מסוים.

    **פתקים** סינכרון הסיסמה נכשל אם סינכרון הסיסמה המוצלח האחרון היה לפני זמן מה.

לקבלת עזרה נוספת לפתרון בעיות בסינכרון סיסמאות, ראה [פתרון בעיות בסינכרון hash של סיסמה עם סינכרון התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).