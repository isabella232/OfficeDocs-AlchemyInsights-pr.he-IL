---
title: צמצם את הבעיה היישום לא אותר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666979"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>צמצם את הבעיה "היישום לא אותר"

שגיאת התקנת היישום, "היישום לא אותר לאחר שההתקנה הושלמה בהצלחה", שדווחה על-ידי Intune, עשויה להופיע בכל פלטפורמות מערכות ההפעלה המרכזיות (Windows, iOS ו- Android).

התרחישים הנפוצים ביותר שמפיקים שגיאה זו כוללים:

- האפליקציה עודכנה מחוץ ל- Intune (מחנות יישומים של ספקים חיצוניים) לאחר הפריסה הראשונית. לדוגמה, יישומים מסוימים, כגון Google Chrome, יכולים לבצע עדכונים אוטומטיים.
- משתמש הסיר את התקנת היישום לאחר ההתקנה הראשונית.

כדי לצמצם את הבעיה, תחילה בצע סקירה של המכשירים המושפעים כדי לקבוע את התרחיש שבו מתרחשת השגיאה.

- אם היישום עודכן מחוץ ל- Intune, ניתן להגדיר את פריסת היישום כך שתתעלם מהגירסה של היישום. כדי לעשות זאת, תחת **'תצורת היישום' > 'מידע על היישום'**, קבע את התכונה **'התעלם מגירסת היישום'** ל **'כן'**.
- כאשר היעד הוא הלקוח, מומלץ להגדיר את היישום כ"נדרש", ולוודא שנפרסת הגירסה העדכנית ביותר.
- לחלופין, בפלטפורמת iOS, ניתן להשתמש בפונקציונליות **AutoUpdate** המשויכת לתוכנית הרכישה בכמות גדולה, אשר את תצורתה ניתן לקבוע לעדכון אוטומטי לגירסאות יישומים חדשות כאשר הן הופכות לזמינות.

לקבלת מידע נוסף על פתרון בעיות בהתקנת יישומים, ראה [פתרון בעיות בהתקנת יישומים](https://docs.microsoft.com/intune/troubleshoot-app-install).
