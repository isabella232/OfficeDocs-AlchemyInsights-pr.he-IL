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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709228"
---
# <a name="content-search-not-returning-expected-results"></a>חיפוש תוכן לא מחזיר תוצאות צפויות

בעת הפעלת חיפושי תוכן מתוך מרכז התאימות של Microsoft 365 _ אמפר _, ייתכן שתקבל תוצאות חיפוש בלתי צפויות. שקול את הדברים הבאים שיכולים להשפיע על תוצאות החיפוש שלך:

- **מיקומי תוכן ותנאי חיפוש**: ודא שבחרת את מיקומי התוכן ותנאי החיפוש המתאימים. אם הרצת חיפוש גדול (עם מיקומים רבים), שקול לפצל אותו לחיפושים מרובים.

- **פריטים בעלי אינדקס חלקי**: פריטים בעלי [אינדקס חלקי](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) מתיבות דואר נכללים בתוצאות החיפוש המשוערות. עם זאת, פריטים הכלולים באינדקס חלקי מאתרים ב-SharePoint ו-OneDrive אינם נכללים בהערכת החיפוש.

- **כשלים בחיפוש**: בעת חיפוש במספר רב של תיבות דואר (מעל 100,000 תיבות דואר), ייתכן שתקבל שגיאות חיפוש, עם קודי שגיאה כגון CS008-009 ו-CS012-002). במקרה זה, נסה שנית לבצע את החיפוש רק עבור מיקומי התוכן שנכשלו. לקבלת מידע נוסף, עיין [במאמר זה](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
