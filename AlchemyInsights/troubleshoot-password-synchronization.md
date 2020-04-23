---
title: פתרון בעיות בסנכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732511"
---
# <a name="troubleshoot-password-synchronization"></a>פתרון בעיות בסנכרון סיסמאות

כדי לפתור בעיות שבהן לא מסונכרנים סיסמאות עם הגירסה 1.1.614.0 או גירסאות מאוחרות יותר של התכונה:
  
1. פתח הפעלה חדשה של Windows PowerShell בשרת החיבור שלך בתכלת AD עם **הפעלת האפשרות מנהל** .

2. הפעלה של **מדיניות הגדרת המדיניות חתומה** או **מוגדרת על-ידי מדיניות בלתי מוגבלת**.

3. הפעל את אשף התקשרות תכלת.

4. נווט לדף **פעילויות נוספות** , בחר **בפתרון בעיות**ולחץ על **הבא**.

5. בדף פתרון בעיות, לחץ על **הפעלה כדי להפעיל את תפריט פתרון התקלות** ב-PowerShell.

6. בתפריט הראשי, בחר **בפתרון בעיות בסינכרון סיסמאות**.

7. בתפריט המשנה, בחר באפשרות **סינכרון סיסמה אינו פועל כלל**.

**הכרת התוצאות של משימת פתרון התקלות**
  
משימת פתרון התקלות מבצעת את הבדיקות הבאות:
  
- מאמת שתכונת סינכרון הסיסמאות מאופשרת עבור דייר ה-"תכלת לספירה" שלך.

- מאמת כי שרת החיבור של תכלת AD אינו במצב אחסון זמני.

- עבור כל מחבר פעיל מקומי של Active Directory (התואם ליער Active Directory קיים):

- 
  - אימות שתכונת סינכרון הסיסמאות מאופשרת.

  - מחפש אירועי פעימה של סינכרון סיסמאות ביומני האירועים של יישום Windows.

  - עבור כל קבוצת מחשבים של Active Directory תחת המחבר Active Directory המקומי:

  - מאמת שניתן להגיע לתחום משרת החיבור של תכלת.

  - מאמת שלחשבונות המשמשים את שירותי התחום של Active Directory (AD DS) שבשימוש מחבר הספריה המקומי יש את שם המשתמש, הסיסמה וההרשאות הדרושים לסנכרון סיסמאות.

לקבלת עזרה נוספת לפתרון בעיות בסינכרון הסיסמה, ראה [פתרון בעיות בסינכרון סיסמאות באמצעות סינכרון התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  