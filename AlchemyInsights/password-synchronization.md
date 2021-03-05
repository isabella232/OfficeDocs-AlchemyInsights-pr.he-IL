---
title: סינכרון סיסמאות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482035"
---
# <a name="password-synchronization"></a>סינכרון סיסמאות

**סינכרון Hash של סיסמאות אינו פועל כלל**

מספר בעיות נפוצות לקוחות מתקיימים כאשר סינכרון Hash של סיסמאות אינו פועל:

- החשבון של Active Directory המשמש את הקישור תכלת AD לתקשורת עם Active Directory מקומי אינו מקבל **שינויי שינויים במדריך** הכתובות **והשכפול של ספריות משנה את כל** ההרשאות, הנדרשות לסינכרון סיסמאות-עליך לתקן זאת על-ידי הענקת הרשאות אלה לחשבון Active Directory.
- סינכרון hash של סיסמאות אינו זמין לאחר שמנהל מערכת שינה את שיטת המשתמש Sign-In **מסינכרון סיסמאות** לאפשרות אחרת, כגון **איחוד עם AD FS** באשף ההתחברות של ' תכלת לספירה '-באפשרותך לפתור זאת על-ידי הפיכת התכונה ' **סינכרון hash של סיסמה** ' לזמינה באשף ההתחברות של ' תכלת ad '.
- בעיית קישוריות עם Active Directory מקומי. לדוגמה, בקרי תחומים מסוימים אינם נגישים על-ידי ' תכלת לספירה ', או [שהיציאות הנדרשות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) נחסמות על-ידי חומת האש-עליך לפתור זאת על-ידי הבטחת הקישוריות בין שרת החיבור של תכלת לספירה לבין active Directory המקומי פועלת כהלכה.
- שרתי הקישור תכלת לספירה הנמצאת כעת במצב האחסון הזמני, שיגרום לכך שהשרת לא יוכל להשתמש בקודי hash של סיסמה-כדי לפתור את הבעיה, בצע את השלבים המתוארים בסעיף [פתרון בעיות בסינכרון סיסמאות עם סינכרון מהדורת תכלת-אין סיסמאות מסונכרנות](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**סינכרון Hash של סיסמאות אינו פועל עבור חלק מהמשתמשים שלי**

1. אם הבחנת ש-hash של סיסמה אינו מסתנכרן עבור משתמש, השתמש במשימה **פתרון בעיות** ב-תכלת AD Connect כדי לחקור ולפתור את הבעיה. בצע את המשימות הבאות:

    מ. [ההפעלה של משימת פתרון הבעיה באשף](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [שימוש ב-cmdlet של פתרון בעיות כדי לבדוק את בעיית סינכרון ה-hash של הסיסמה לשימוש ספציפי](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. אובייקט המשתמש המקומי של Active Directory זמין עבור **המשתמש כדי לשנות את הסיסמה באפשרות הכניסה הבאה** . כאשר אפשרות זו זמינה, המשתמש מוקצה לסיסמה זמנית והוא יתבקש לשנות את הסיסמה בכניסה הבאה. חיבור תכלת לספירה אינו מסנכרן סיסמאות זמניות לתכלת לספירה.

כדי לפתור את הבעיה לעיל, בצע אחת מהמשימות הבאות:

- בקש מהמשתמש להיכנס ליישום מקומי (לדוגמה, שולחן העבודה של Windows) ולשנות את הסיסמה. הסיסמה החדשה תסונכרן לכיוון תכלת לספירה.
- מנהל מערכת עדכן את סיסמת המשתמש מבלי להפוך את האפשרות של **משתמש לזמינה לשנות את הסיסמה בכניסה הבאה** ולשתף את הסיסמה החדשה עם המשתמש.

3. אובייקט המשתמש המקומי של Active Directory **אינו מוגדר כהלכה** עבור סינכרון אובייקטים או סינכרון סיסמאות. כדי לפתור בעיה זו, בצע את השלבים המתוארים [בסינכרון ה-hash של הסיסמה לפתרון בעיות בסינכרון של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







