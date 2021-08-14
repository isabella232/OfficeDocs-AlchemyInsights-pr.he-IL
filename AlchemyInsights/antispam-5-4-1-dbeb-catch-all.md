---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932278"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>פתרון בעיות מסירה עבור קוד שגיאה 550 5.4.1 ממסר Access נדחה

בעיה זו מתרחשת [בעת בדיקה אם כתובת דואר אלקטרוני חוקית כדי למנוע החזרים חוזרים](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) בעת הזנת רשת Microsoft. נסה את הפעולות הבאות:

1. קבע אם הבעיה ספציפית לתחום שלם או לכתובת דואר אלקטרוני בודדת:
    - התחום כולו: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום ל'פנימי' ולאחר מכן לחזור ל' סמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - כתובת דואר אלקטרוני בודדת: לפעמים יש לסנכרן את הכתובת; שינוי כתובת ה- Proxy של smtp ולאחר מכן שינוי כתובת ה- Proxy יכול לעזור.
2. קבע אם הבעיה ספציפית לקבוצה או לתיקיה ציבורית. עבור סוגי אובייקטים מסוימים, ייתכן שיהיה צורך ליצור את האובייקטים באופן ידני ב- Azure Active Directory.

אם אתה זקוק לעזרה נוספת, פתח כרטיס תמיכה וציין את היקף הבעיה (כולל סוג האובייקט שאתה שולח לו) כדי שנוכל לסייע לך טוב יותר.