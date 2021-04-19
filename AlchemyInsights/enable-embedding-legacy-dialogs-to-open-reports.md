---
title: הפיכת הטבעה של תיבות דו-שיח מדור קודם לזמינה כדי לפתוח דוחות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814265"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>הפיכת הטבעה של תיבות דו-שיח מדור קודם לזמינה כדי לפתוח דוחות

**מאפיין הבעיה**

למשתמשים אין אפשרות לפתוח דוחות. "משהו השתבש. עיין בפרטים הטכניים לקבלת פרטים נוספים."

**סיבה**

הדוחות נכשלים בטעינה ב- UCI עם השגיאה "Form מתאר הוא Null או לא מוגדר". דוחות ב- UCI עדיין דורשים תיבות דו-שיח מדור קודם, כך שמערכת הלקוח צריכה לאפשר שימוש ב- *allowlegacydialogsembedding.*

**פתרון**

1. עבור אל **הגדרות >ניהול > הגדרות > כללי**.

2. הגדר "אפשר הטבעה של תיבות דו-שיח מדור קודם מסוימות בלקוח דפדפן Unified Interface" **ל'כן'.**
