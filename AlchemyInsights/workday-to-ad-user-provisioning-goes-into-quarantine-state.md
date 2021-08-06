---
title: יום עבודה להקצאת משתמשים של AD עובר למצב הסגר
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
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036493"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>יום עבודה להקצאת משתמשים של AD עובר למצב הסגר

**יום עבודה להקצאת משתמשים של AD עובר למצב ההסגר ולא נוצרים משתמשים ב- AD**

המשימה הקצאת משאבים למשתמשי עבודה ל- AD חלפה למצב ההסגר ויומני הביקורת מציגים אירועי כשל ייצוא עם הודעת **השגיאה: OperationsError-SvcErr: אירעה שגיאת פעולה. לא הוגדרה הפניה נעלה עבור שירות מדריך הכתובות. לכן, לשירות מדריך הכתובות אין אפשרות להנפיק הפניות לאובייקטים מחוץ ליער זה.** שגיאה זו מופיעה בדרך כלל אם ה- OU של הגורם המכיל של Active Directory אינו מוגדר כראוי או אם ייתנו בעיות במיפוי הביטויים המשמש עבור **parentDistinguishedName**.

בדוק את הפרמטר OU **המהווה ברירת מחדל עבור משתמשים** חדשים עבור שגיאות הקלדה. ודא שה- OU שצוין כבר קיים ב- AD. אם אתה משתמש **ב- parentDistinguishedName** במיפוי התכונות, ודא שהוא מוערך תמיד כגורמים מכילים ידועים בתחום AD. בדוק את האירוע ייצוא ביומני הביקורת כדי לראות את הערך שנוצר.

לקבלת פרטים נוספים אודות קביעת התצורה של יום עבודה להקצאה אוטומטית, ראה [ערכת לימוד: קביעת תצורה של יום עבודה להקצאת משתמשים אוטומטית.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

