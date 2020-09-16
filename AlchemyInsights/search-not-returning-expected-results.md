---
title: 1491-חיפוש-לא-חוזר-התוצאות הצפויות
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740475"
---
# <a name="content-search-not-returning-expected-results"></a>חיפוש תוכן אינו מחזיר תוצאות צפויות

בעת הפעלת חיפושי תוכן ממרכז התאימות של Microsoft 365 security &, ייתכן שתקבל תוצאות חיפוש בלתי צפויות. שקול את הדברים הבאים העשויים להשפיע על תוצאות החיפוש:

- **מיקומים ותנאי חיפוש של תוכן**: ודא שבחרת את מיקומי התוכן המתאימים ותנאי חיפוש. אם הפעלת חיפוש גדול (עם מיקומים רבים), שקול לפצל אותו לחיפושים מרובים.

- **פריטים הכלולים באינדקס באופן חלקי**: פריטים הכלולים  [באינדקס באופן חלקי](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) מתיבות דואר כלולים בתוצאות החיפוש המוערכות. עם זאת, פריטים הכלולים באינדקס באופן חלקי מאתרים ב-SharePoint ו-OneDrive אינם כלולים בהערכת החיפוש.

- **כשלים בחיפוש**: בעת חיפוש מספר גדול של תיבות דואר (מעל לתיבות דואר של 100,000), אתה עשוי לקבל שגיאות חיפוש, עם קודי שגיאה כגון CS008-900 ו-CS012-002). במקרה זה, נסה שוב לבצע את החיפוש עבור מיקומי התוכן שכשלו. עיין  [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) לקבלת מידע נוסף.
