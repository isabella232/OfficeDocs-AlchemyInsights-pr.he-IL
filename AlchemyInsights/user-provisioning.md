---
title: הקצאת משתמשים
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971340"
---
# <a name="user-provisioning"></a>הקצאת משתמשים

- השתמש ביכולת [הקצאת המשאבים לפי דרישה](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) כדי להקצות משתמש לקבלת אבחון מפורט אודות השלבים המפורטים.
- כדי לפתור בעיות שאתה נתקל בהן בעת הקצאת משאבים למשתמשים ולקבוצות, עיין במדריך [לפתרון בעיות לא הוקצה למשתמשים.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- אם אתה מבחין שלא הוקצו משאבים למשתמשים, ראה הקצאת משאבים של יומני [רישום (תצוגה מקדימה) ב-](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) Azure Active Directory (AD). חפש ערכי יומן רישום הקשורים למשתמש ספציפי.
- הפעלה מחדש מעת לעת של הקצאת משאבים כדי לתפוס את כל המשתמשים שלא נענו במחזור הקצאת משאבים קודם.
- ייתכן שהמשתמש/הקבוצה לא הוקצו מאחר שהשירות שלנו עדיין לא בחן את המשתמש. סקור את ההנחיות לגבי הזמן שנדרש להקצאה וכן את מד ההתקדמות בדף קביעת התצורה של הקצאת המשאבים. אם המצב היציב שצוין במקטע פרטים נוספים הוא לפני התאריך שהמשתמש נוצר/עודכן/נמחק, פירוש הדבר שלא הערכנו את המשתמש עדיין. בתרחיש זה, הדבר הטוב ביותר לעשות הוא להמתין עד ששירות הקצאת המשאבים יסיים. אם המצב היציב הושג, מומלץ לבצע הפעלה מחדש מתוך ממשק המשתמש בפורטל Azure.
  - שים לב שהשירות שלנו מודע רק לשינויים במשתמש/קבוצה במערכת המקור (Azure Active Directory). אם משתמש/קבוצה מוסר ישירות ביישום (לדוגמה, ServiceNow), איננו מודעים לשינויים אלה ולא חוזרים על סמך מצב המשתמש במערכת המקור. בתרחיש זה, הכי טוב להחזיר את השינוי ישירות ביישום היעד.
- השירות שלנו העריך את המשתמש/הקבוצה וקבע שלא ניתן להקצות אותו:
  - אם הגדרת את הטווח למשתמשים ולקבוצות מוקצים, בדוק אם המשתמש/הקבוצה מוקצה ליישום.
  - אם המשתמש/הקבוצה מוקצה ליישום, ודא שהם אינם מוקצים לתפקיד הגישה המוגדר כברירת מחדל. לא ניתן להשתמש בתפקיד זה להקצאת משאבים.
  - אם הגדרת מסנן scoping מבוסס תכונה, ודא שהמשתמש יתקוף את הקריטריונים שציינת.
  - אם משתמשים כבר קיימים במערכת היעד ובמדינה של המשתמש בהתאמה למקור וליעד, לא נ לנקוט פעולה נוספת.
- השירות שלנו ניסה להקצות את המשתמש והוא נכשל. עבור תרחישים אלה, עיין בכרטיסיה פתרון בעיות והמלצות של יומני הקצאת המשאבים:
  - ייתכן שתכונה נדרשת למשתמש חסרה ב- Azure Active Directory או אינה תואמת לתבנית הנדרשת על-ידי יישום צד שלישי. לדוגמה, התכונה מדינה על משתמש עשויה להיות מוגדרת לארצות הברית כאשר היא אמורה להיות ארה"ב.
  - התכונה היא תכונת הקשרים הקיימת עדיין ביישום היעד. תכונת הקשרים היא תכונה שמצביעה על אובייקט אחר, לדוגמה, משתמש שהוא חבר בקבוצה. מזהה המשתמש יהיה בתכונת החבר של הקבוצה, אך ניתן לעבד אותו רק אם אובייקט המשתמש שהוא מצביע עליו כבר קיים.
