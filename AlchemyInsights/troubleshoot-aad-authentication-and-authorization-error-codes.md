---
title: פתרון בעיות בקודי שגיאה של אימות מודעות מיידיות ואישורים (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036506"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>פתרון בעיות בקודי שגיאה של אימות מודעות מיידיות ואישורים (AADSTS)

כדי לפתור את האימות או קודי שגיאת ההרשאות של AADSTS, בצע את השלבים המומלצים הבאים:

1. **טיפול בקודי שגיאה ביישום**

- **Oauth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 מספק הנחיות לטיפול בשגיאות במהלך אימות באמצעות חלק השגיאה של תגובת השגיאה.

    - **שגיאה**: מחרוזת קוד שגיאה שניתן להשתמש בה כדי לסווג סוגים של שגיאות שמתרחשות, ויש להשתמש בהם כדי להגיב לשגיאות.
    - שדה **השגיאה** מכיל כמה ערכים אפשריים-סקור את קישורי תיעוד הפרוטוקול ומפרט OAuth 2.0 לקבלת מידע נוסף אודות שגיאות ספציפיות וכיצד להגיב להן.

- להלן תגובת שגיאה לדוגמה:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **מידע אודות קוד השגיאה הנוכחי של בדיקת מידע**

- קודי שגיאה והודעות כפופים לשינוי. לקבלת המידע העדכני ביותר, עיין https://login.microsoftonline.com/error בעמוד כדי למצוא את תיאורי השגיאות, התיקונים והפתרונות המוצעים של AADSTS.
- באפשרותך גם לחפש [קודי שגיאה של AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) ולפתור בעיות המפורטים במאמר [תכלת לספירה וקודי שגיאה של מתן הרשאות](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **קבלת עזרה**

- [אפשרויות תמיכה ועזרה עבור מפתחים](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -אם אתה זקוק לתשובה לשאלה או לעזרה בפתרון בעיה שאינה מכוסה בתיעוד שלנו, ייתכן שהגיע הזמן להושיט יד למומחים לקבלת עזרה. מאמר זה מספק כמה הצעות לקבלת תשובות לשאלות שלך בעת פיתוח יישומים המשולבים עם פלטפורמת הזהות של Microsoft.








