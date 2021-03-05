---
title: יום עבודה לפרסום הקצאת משתמשים נכנסת למצב הסגר
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481875"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>יום עבודה לפרסום הקצאת משתמשים נכנסת למצב הסגר

**יום עבודה כדי להעביר הקצאת משתמשים נכנסת למצב הסגר ולא נוצרות משתמשים ב-AD**

משימת הקצאת המשאבים למשתמש של יום העבודה עברה למצב ההסגר ויומני הביקורת מראים אירועי כשל ייצוא עם שגיאת הודעת השגיאה **: OperationsError-SvcErr: אירעה שגיאת פעולה. לא הוגדרו הפניה מעולה עבור שירות מדריך הכתובות. לפיכך, שירות מדריך הכתובות אינו מצליח להנפיק הפניות לאובייקטים מחוץ ליער זה**. שגיאה זו בדרך כלל מופיעה אם הגורם המכיל של Active Directory אינו מוגדר כהלכה או אם קיימות בעיות במיפוי הביטויים המשמש **parentDistinguishedName**.

סמן את הפרמטר OU המוגדר כברירת מחדל עבור **משתמשים חדשים** עבור הקלדה. ודא שה-OU שצוין כבר קיים במודעה שלך. אם אתה משתמש ב- **parentDistinguishedName** במיפוי התכונות, ודא שהוא תמיד מוערך כגורם מכיל מוכר בתוך התחום המודע. סמן את אירוע הייצוא ביומני הביקורת כדי לראות את הערך שנוצר.

לקבלת פרטים נוספים על קביעת התצורה של יום העבודה לצורך הקצאה אוטומטית, ראה [ערכת לימוד: קביעת התצורה של יום עבודה עבור הקצאת משתמשים אוטומטית](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

