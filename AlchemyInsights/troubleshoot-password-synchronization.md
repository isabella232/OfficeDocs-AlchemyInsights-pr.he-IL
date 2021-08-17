---
title: פתרון בעיות סינכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105752"
---
# <a name="troubleshoot-password-synchronization"></a>פתרון בעיות סינכרון סיסמאות

כדי לפתור בעיות סינכרון סיסמאות, התחל על-ידי שימוש במשימה זו התחברות פתרון בעיות כדי לקבוע מדוע סיסמאות לא מסתנכרנים. כדי להתחיל, עבור אל [ניהול סינכרון ישיר](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. פתח הפעלת Windows PowerShell חדשה בשרת Azure AD התחברות, ובחר באפשרות **הפעל כמנהל** מערכת.

2. הפעל Set-ExecutionPolicy RemoteSigned או Set-ExecutionPolicy בלתי מוגבל.

3. הפעל את אשף התחברות Azure AD.

4. עבור אל הדף משימות נוספות כדי > **פתרון**  >  **בעיות הבא**.

5. בחר **הפעל כדי** לפתוח את תפריט פתרון הבעיות של PowerShell.

6. בחר **פתרון בעיות סינכרון סיסמאות**.

    הבעיה היא בדרך כלל שסיסמה אינה מסונכרנת עבור חשבון משתמש ספציפי.

    **הערות** סינכרון סיסמאות נכשל אם סינכרון הסיסמה המוצלח האחרון היה לפני זמן מה.

לקבלת עזרה נוספים בפתרון בעיות בסינכרון סיסמאות, ראה [פתרון בעיות בסינכרון hash של סיסמאות עם Azure AD התחברות סינכרון](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).