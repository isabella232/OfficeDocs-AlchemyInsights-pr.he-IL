---
title: 1491-search-not-returning-expected-results
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052711"
---
# <a name="content-search-not-returning-expected-results"></a>חיפוש תוכן אינו מחזיר תוצאות צפויות

בעת הפעלת חיפושי תוכן ממרכז Microsoft 365 האבטחה &, ייתכן שתקבל תוצאות חיפוש בלתי צפויות. שקול את הדברים הבאים ה יכולים להשפיע על תוצאות החיפוש שלך:

- **מיקומי תוכן ותנאי** חיפוש : ודא שבחרת את מיקומי התוכן והתנאי החיפוש המתאימים. אם הרצת חיפוש גדול (עם מיקומים רבים), שקול לפצל אותו לחיפושים מרובים.

- **פריטים הכלולים באינדקס** חלקית: פריטים שכלולים  [באינדקס](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) חלקית מתיבות דואר כלולים בתוצאות החיפוש המשוערות. עם זאת, פריטים הכלולים באינדקס חלקית מהאתרים SharePoint ופריטים OneDrive אינם כלולים בהערכת החיפוש.

- **כשלי חיפוש**: בעת חיפוש במספר גדול של תיבות דואר (מעל 100,000 תיבות דואר), ייתכן ותתרחש שגיאות חיפוש, עם קודי שגיאה כגון CS008-009 ו- CS012-002). במקרה זה, נסה שוב לחפש רק את מיקומי התוכן שנכשלו. עיין  [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) לקבלת מידע נוסף.
