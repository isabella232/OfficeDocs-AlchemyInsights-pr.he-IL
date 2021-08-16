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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003390"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>הפיכת הטבעה של תיבות דו-שיח מדור קודם לזמינה כדי לפתוח דוחות

**מאפיין הבעיה**

למשתמשים אין אפשרות לפתוח דוחות. "משהו השתבש. עיין בפרטים הטכניים לקבלת פרטים נוספים."

**סיבה**

הדוחות נכשלים בטעינה ב- UCI עם השגיאה "Form מתאר הוא Null או לא מוגדר". דוחות ב- UCI עדיין דורשים תיבות דו-שיח מדור קודם, כך שמערכת הלקוח צריכה לאפשר שימוש ב- *allowlegacydialogsembedding.*

**פתרון**

1. עבור אל **הגדרות >ניהול > מערכת הגדרות > כללי**.

2. הגדר "אפשר הטבעה של תיבות דו-שיח מדור קודם מסוימות בלקוח דפדפן Unified Interface" **ל'כן'.**
