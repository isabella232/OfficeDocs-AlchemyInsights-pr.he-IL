---
title: בעיות בהסכמת מנהל מערכת
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952574"
---
# <a name="admin-consent-issues"></a>בעיות בהסכמת מנהל מערכת

1. הפוך את [זרימת העבודה של הסכמת מנהל](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) מערכת לזמינה כדי לאפשר למשתמשים לבקש אישור מנהל מערכת ישירות ממסך ההסכמה.

1. אם אתה או משתמשי היישום שלך רואים שגיאות בלתי צפויות במהלך תהליך ההסכמה, עיין במאמר זה לקבלת שלבים לפתרון בעיות: שגיאה בלתי [צפויה בעת ביצוע הסכמה ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. קבל מידע נוסף [על הסכמת מנהל מערכת](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) פלטפורמת הזהויות של Microsoft , כיצד פועלת בקשת ההסכמה ואופן ההערכה של בקשה [להסכמת מנהל מערכת כלל-דייר.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. יישומים שמשתלבים עם פלטפורמת הזהויות של Microsoft עוקבים אחר מודל הרשאה המעניק למשתמשים ולמנהלי מערכת שליטה באופן הגישה לנתונים. היישום של מודל ההרשאות עודכן בנקודות הקצה פלטפורמת הזהויות של Microsoft, והוא משנה את האופן בו יישום חייב לקיים אינטראקציה עם פלטפורמת הזהויות של Microsoft. ראה [הרשאות והסכמה בנקודות פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) לקבלת מבט כולל על מודל הרשאה זה, כולל טווחים, הרשאות והסכמה.