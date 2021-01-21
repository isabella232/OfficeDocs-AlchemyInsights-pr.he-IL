---
title: קביעת תצורה והארכה של אורך חיים של אסימונים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916827"
---
# <a name="configure-and-extend-token-lifetimes"></a>קביעת תצורה והארכה של אורך חיים של אסימונים

באפשרותך לציין את אורך החיים של האסימון access, SAML או ID שהונפק על-ידי פלטפורמת הזהות של Microsoft. באפשרותך להגדיר אורך חיים של אסימונים עבור כל היישומים בארגון שלך, עבור יישום רב-דייר (מרובה ארגונים), או עבור מנהל שירות ספציפי בארגון שלך. לקבלת מידע נוסף, קרא [אורך חיים של אסימונים הניתנים להגדרה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

לקבלת דוגמאות, קרא [דוגמאות לאופן הגדרת אורך חיים של אסימונים](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

כדי ללמוד כיצד להגדיר את משך החיים והתאימות של אסימון בתכלת Active Directory B2C (תכלת AD B2C), ראה [קביעת תצורה של אסימונים בתכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

המאמר [קביעת התצורה של אופן הפעולה של הפעלה ב-תכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) מתאר את שיטות הכניסה היחידה (SSO) המשמשות ב-תכלת AD B2C ועוזר לך לבחור את שיטת ה-sso המתאימה ביותר בעת קביעת התצורה של המדיניות שלך.

**כמה זמן יימשך אסימונים? לכמה זמן הם תקפים?**

אורך חיים של אסימונים הוא שעה והמשך הזמן של ההפעלה הוא 24 שעות. משמעות הדבר היא שאם לא בוצעו בקשות ב-24 שעות, יהיה עליך להיכנס שוב לפני בקשת אסימון חדש.

> [!NOTE]
> לאחר 30 במאי 2020, אף דייר חדש לא יוכל להשתמש במדיניות לכל החיים של אסימונים הניתנים להגדרה כדי לקבוע את התצורה של אסימוני הפעלה ורענון. התבטלות יקרה תוך מספר חודשים לאחר מכן, כלומר, נפסיק לכבד הפעלה קיימת ונרענן משטרת אסימונים. עדיין ניתן לקבוע את התצורה של אורך חיים של אסימון גישה לאחר תבטלות.






