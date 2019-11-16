---
title: 5.4.1 האנטי ספאם לתפוס-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672434"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>תקן בעיות מסירה עבור קוד שגיאה 550 5.4.1 ממסר גישה נדחתה

בעיה זו [מתרחשת בעת בדיקה כדי לבדוק אם כתובת דואר אלקטרוני היא חוקית כדי למנוע](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) הסגת זמן בעת הכניסה לרשת של Office 365. נסה את הפעולות הבאות:

1. קבע אם הבעיה היא ספציפית לתחום שלם או לכתובת דואר אלקטרוני יחידה:
    - כל התחום: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום כפנימי ולאחר מכן לחזור לסמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - כתובת דוא ל יחידה: לעתים יש לסנכרן את הכתובת; שינוי כתובת ה-proxy של smtp ולאחר מכן שינוי החזרה יכול לעזור.
2. קבע אם הבעיה היא ספציפית לקבוצה או לתיקיה ציבורית. עבור סוגי אובייקטים מסוימים, ייתכן שיהיה צורך ליצור את האובייקטים באופן ידני באמצעות הספריה הפעילה.

אם אתה זקוק לעזרה נוספת, נא פתח כרטיס תמיכה וציין את היקף הבעיה (כולל את סוג האובייקט שאתה שולח ל) כדי שנוכל לסייע לך בצורה טובה יותר.