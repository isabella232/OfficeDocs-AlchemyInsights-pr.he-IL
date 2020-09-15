---
title: 5.4.1 DBEB לתפוס את כל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717362"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>פתרון בעיות במסירה עבור קוד שגיאה 550 הגישה של 5.4.1 ממסר נדחתה

בעיה זו מתרחשת בעת [בדיקה אם כתובת דואר אלקטרוני חוקית כדי למנוע את bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) בעת הכניסה לרשת Microsoft. נסה את הפעולות הבאות:

1. קבע אם הבעיה ספציפית לתחום כולו או לכתובת דואר אלקטרוני אחת:
    - תחום כולו: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום לפנימי ולאחר מכן לחזור לסמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - כתובת דואר אלקטרוני יחידה: לפעמים צריך לסנכרן את הכתובת; שינוי כתובת ה-proxy של smtp ולאחר מכן שינוי שלו בחזרה יכול לעזור.
2. קביעה אם הבעיה ספציפית לקבוצה או לתיקיה ציבורית. עבור סוגי אובייקטים מסוימים, ייתכן שיהיה עליך ליצור את האובייקטים באופן ידני ב-תכלת Active Directory.

אם אתה זקוק לעזרה נוספת, פתח כרטיס תמיכה וציין את טווח הבעיה (כולל סוג האובייקט שאליו אתה שולח) כדי שנוכל לסייע לך בצורה טובה יותר.