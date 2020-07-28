---
title: מלאי מכשירים Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439654"
---
# <a name="intune-device-inventory"></a>מלאי מכשירים Intune

הלהב Devices מספק את התובנה של מנהל מערכת בהתקנים תחת ניהול ב-Intune על בסיס כל התקן. המידע המוצג כולל: חומרה, יישומים שהתגלו, מצב תאימות התקנים ומצב תצורת התקן.

נתוני מלאי עבור חומרה ויישומים שהתגלו נאספים במחזור של שבעה ימים. היישומים והרכיבים הספציפיים של החומרה שדווחו שונים בהתאם למערכת ההפעלה של ההתקן ולשאלה אם ההתקן הוא אישי או בבעלות חברה.

לקבלת מידע נוסף, ראה [ראה פרטי התקן ב-Intune](https://docs.microsoft.com/intune/device-inventory).

**שאלות נפוצות**

ש: אני לא מקבל רשימת מלאי מלאה של יישומים הנמצאים בIntune התקנים של Windows שנרשמו. למה לא?

ת: בשלב זה, רק אפליקציות מודרניות מפורטות עבור Windows 10 PCs המזוהים כהתקנים ארגוניים. Intune אינו אוסף מידע אודות יישומי Win32 המותקנים במכשירים אלה.

ש: מדוע לא נאספים מספרי טלפון מכל המכשירים?

ת: טלפונים המסווגים כהתקנים ארגוניים ב-Intune אינם מזוהים עם מספר הטלפון המלא שלהם כאשר, לדוגמה, אתה מפעיל דוח מלאי של התקן נייד. מספרי טלפון בהתקן הבא-לך-התקן מוסתרים תמיד באופן חלקי עם כוכביות (* * * *) ומציגות רק את ארבע הספרות האחרונות.