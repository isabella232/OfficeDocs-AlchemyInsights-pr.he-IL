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
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821448"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>פתרון בעיות מסירה עבור קוד שגיאה 550 5.4.1 ממסר Access נדחה

בעיה זו מתרחשת [בעת בדיקה אם כתובת דואר אלקטרוני חוקית כדי למנוע החזרים חוזרים](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) בעת הזנת רשת Microsoft. נסה את הפעולות הבאות:

1. קבע אם הבעיה ספציפית לתחום שלם או לכתובת דואר אלקטרוני בודדת:
    - התחום כולו: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום ל'פנימי' ולאחר מכן לחזור ל' סמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - כתובת דואר אלקטרוני בודדת: לפעמים יש לסנכרן את הכתובת; שינוי כתובת ה- Proxy של smtp ולאחר מכן שינוי כתובת ה- Proxy יכול לעזור.
2. קבע אם הבעיה ספציפית לקבוצה או לתיקיה ציבורית. עבור סוגי אובייקטים מסוימים, ייתכן שיהיה צורך ליצור את האובייקטים באופן ידני ב- Azure Active Directory.

אם אתה זקוק לעזרה נוספת, פתח כרטיס תמיכה וציין את היקף הבעיה (כולל סוג האובייקט שאתה שולח לו) כדי שנוכל לסייע לך טוב יותר.