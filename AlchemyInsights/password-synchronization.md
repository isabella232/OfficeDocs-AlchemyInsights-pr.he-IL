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
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960836"
---
# <a name="password-synchronization"></a>סינכרון סיסמאות

**סינכרון Hash של סיסמה אינו פועל כלל**

כמה בעיות נפוצות שהלקוחות נתקלים בהן כאשר סינכרון Hash של סיסמה אינו פועל הן:

- חשבון Active Directory המשמש את Azure AD התחברות כדי לקיים תקשורת עם  Active Directory  מקומי אינו מוענק לשכפול שינויים במדריך הכתובות ושכפול שינויים במדריך הכתובות כל ההרשאות הדרושות לסינכרון סיסמאות - עליך לתקן זאת על-ידי הענקת הרשאות אלה לחשבון Active Directory.
- סינכרון Hash של סיסמאות אינו זמין לאחר שמנהל  מערכת שינה את שיטת המשתמש Sign-In מסינכרון סיסמאות לאפשרות אחרת, כגון איחוד עם **AD FS** באשף Azure AD התחברות - באפשרותך לתקן זאת על-ידי הפיכת תכונת סינכרון ה- **Hash** של הסיסמה לאשף Azure AD התחברות.
- בעיית קישוריות ב- Active Directory מקומי. לדוגמה, בקרי תחום מסוימים אינם נגישים על-ידי Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) AD התחברות, או שהיציאות הנדרשות נחסמות על-ידי חומת האש - עליך לתקן זאת על-ידי הבטחת שהקישוריות בין שרת Azure AD התחברות לבין Active Directory המקומי פועלת כראוי.
- שרת Azure AD התחברות נמצא כעת במצב אחסון זמני, דבר אשר יגרום לכך שהשרת לא יוכל לבצע את ה- Hash של הסיסמה - כדי לפתור את הבעיה, בצע את השלבים המתוארים בסעיף פתרון בעיות סינכרון סיסמאות עם סינכרון Azure AD התחברות - לא [מסונכרנות סיסמאות.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**סינכרון Hash של סיסמה אינו פועל עבור חלק מהמשתמשים שלי**

1. אם שמת לב ש- Hash של סיסמה אינו  מסתנכרן עבור משתמש, השתמש במשימה לפתור בעיות ב- Azure AD התחברות כדי לחקור ולפתור את הבעיה. בצע את המשימות הבאות:

    a. [הפעלת המשימה לפתרון בעיות באשף](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [השתמש ב- cmdlet לפתרון בעיות כדי לחקור את בעיית סינכרון קוד ה- Hash של הסיסמה עבור שימוש ספציפי](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. האובייקט המקומי של Active Directory User זמין עבור המשתמש חייב לשנות **סיסמה באפשרות הכניסה** הבאה. כאשר אפשרות זו זמינה, למשתמש מוקצית סיסמה זמנית ותתבקש לשנות את הסיסמה בכניסה הבאה. Azure AD התחברות סינכרון סיסמאות זמניות ל- Azure AD.

כדי לפתור את הבעיה לעיל, בצע אחת מהמשימות הבאות:

- בקש מהמשתמש להיכנס ליישום מקומי (לדוגמה, Windows Desktop) ולשנות את הסיסמה. הסיסמה החדשה תסונכרן עם Azure AD.
- יש למנהל מערכת לעדכן את סיסמת המשתמש מבלי לאפשר את האפשרות המשתמש **חייב לשנות סיסמה** בכניסה הבאה ולשתף את הסיסמה החדשה עם המשתמש.

3. אובייקט המשתמש המקומי של Active Directory אינו מוגדר כראוי **עבור סינכרון אובייקטים** או סינכרון סיסמאות. כדי לפתור בעיה זו, בצע את השלבים המתוארים בפתרון [בעיות סינכרון hash של סיסמאות עם Azure AD התחברות סינכרון](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







