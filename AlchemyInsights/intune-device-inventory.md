---
title: Intune Device Inventory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014073"
---
# <a name="intune-device-inventory"></a>Intune Device Inventory

להב המכשירים מספק למנהל המערכת תובנות לגבי מכשירים תחת ניהול ב- Intune על בסיס כל מכשיר. המידע המוצג כולל: חומרה, יישומים שהתגלו, מצב תאימות מכשיר ומדינה של תצורת מכשיר.

נתוני מלאי עבור חומרה ויישומים שהתגלו נאספים במחזור של שבעה ימים. היישומים ורכיבי החומרה הספציפיים שדווחו משתנים בהתאם למערכת ההפעלה של המכשיר ואם המכשיר נמצא בבעלות אישית או בבעלות ארגונית.

לקבלת מידע נוסף, ראה [ראה פרטי מכשיר ב- Intune](https://docs.microsoft.com/intune/device-inventory).

**שאלות נפוצות**

ש: איני מקבל רשימת מלאי מלאה של יישומים המוצגים במכשירי Intune שנרשמו Windows. למה לא?

ת: בשלב זה, רק אפליקציות מודרניות מפורטות עבור Windows 10 אישיים המזוהים כמכשירים ארגוניים. Intune אינו אוסף מידע אודות יישומי Win32 המותקנים במכשירים אלה.

ש: מדוע מספרי טלפון אינם נאספים מכל המכשירים?

ת: טלפונים מסווגים כמכשירים ארגוניים ב- Intune אינם מזוהים עם מספר הטלפון המלא שלהם כאשר, לדוגמה, אתה מפעיל מלאי של מכשירים ניידים הדוח. מספרי הטלפון של Bring-you-own-device תמיד עם מסיכה חלקית עם כוכביות (****), ומראים רק את ארבע הספרות האחרונות.