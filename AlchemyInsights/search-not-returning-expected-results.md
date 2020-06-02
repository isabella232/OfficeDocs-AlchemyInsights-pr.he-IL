---
title: 1491-חיפוש-לא-חוזר-צפוי-תוצאות
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510573"
---
# <a name="content-search-not-returning-expected-results"></a>חיפוש תוכן לא מחזיר תוצאות צפויות

בעת הפעלת חיפושי תוכן מתוך מרכז התאימות של Microsoft 365 _ אמפר _, ייתכן שתקבל תוצאות חיפוש בלתי צפויות. שקול את הדברים הבאים שיכולים להשפיע על תוצאות החיפוש שלך:

- **מיקומי תוכן ותנאי חיפוש**: ודא שבחרת את מיקומי התוכן ותנאי החיפוש המתאימים. אם הרצת חיפוש גדול (עם מיקומים רבים), שקול לפצל אותו לחיפושים מרובים.

- **פריטים בעלי אינדקס חלקי**: פריטים בעלי [אינדקס חלקי](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) מתיבות דואר נכללים בתוצאות החיפוש המשוערות. עם זאת, פריטים הכלולים באינדקס חלקי מאתרים ב-SharePoint ו-OneDrive אינם נכללים בהערכת החיפוש.

- **כשלים בחיפוש**: בעת חיפוש במספר רב של תיבות דואר (מעל 100,000 תיבות דואר), ייתכן שתקבל שגיאות חיפוש, עם קודי שגיאה כגון CS008-009 ו-CS012-002). במקרה זה, נסה שנית לבצע את החיפוש רק עבור מיקומי התוכן שנכשלו. לקבלת מידע נוסף, עיין [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
