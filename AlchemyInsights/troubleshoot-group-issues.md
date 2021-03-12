---
title: פתרון בעיות בקבוצה
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713645"
---
# <a name="troubleshoot-group-issues"></a>פתרון בעיות בקבוצה

**אני צריך להקצות קבוצה לתפקיד תכלת לספירה**

כדי להקצות קבוצה של תכלת Active Directory (AD) לתפקיד תכלת לספירה, בצע את השלבים הבאים:

1. צור קבוצה חדשה-כדי ליצור קבוצה חדשה:

    מ. היכנס למרכז הניהול של תכלת לספירה עם הרשאות מנהל תפקידים מורשה או מנהל מערכת כללי. 
    b. בחר באפשרות תכלת Active Directory > קבוצות > כל הקבוצות > קבוצה חדשה. 
    c. יצירת הקבוצה.

2. הקצה את התפקיד לקבוצה במהלך יצירת הקבוצה או לאחר יצירת הקבוצה.

    מ. כדי להקצות תפקיד לקבוצה בזמן יצירת הקבוצה, עבור לקבוצה החלפת תפקידים של העברת הודעות מיידיות של תכלת ויצירת הקבוצה.
    b. כדי להקצות תפקיד לקבוצה לאחר יצירתה, נווט אל הכרטיסיה תפקידים שהוקצו עבור הקבוצה החדשה שנוצרה, והקצה את התפקיד לקבוצה.

**אני צריך לנהל את החברות בקבוצה המוקצית לתפקיד המודע של התכלת**

1. כדי למנוע העלאת הרשאות, כברירת מחדל, רק מנהל התפקידים המורשה ומנהל המערכת הכללי יכולים לשנות את החברות של קבוצה שהוקצתה לתפקיד. עם זאת, הם יכולים לבחור להקצות בעלים עבור קבוצה כזו ולהקצות משימה זו. לקבלת מידע נוסף, ראה [שימוש בקבוצות ענן לניהול הקצאות תפקידים ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. לשאלות נפוצות ועצות לפתרון בעיות עבור הקצאת תפקידים לקבוצות ב-תכלת לספירה, ראה [תפקידי פתרון בעיות שהוקצו לקבוצות ענן](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**קבוצות דינמיות**

1. אם אינך מצליח למצוא את תכונות המשתמש המוכללות, ודא שהתכונה נמצאת ברשימת המאפיינים הנתמכים.
2. אם אתה מחפש תכונות מוכללות של מכשירים, ודא שהתכונה נמצאת ברשימת תכונות ההתקן 
3. בנוסף לתכונות המוכללות של המשתמש וההתקן, ניתן גם להשתמש [בתכונות הרחבה](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). לאחר סינכרון תכונות ההרחבה מתוך מקומי Windows Server AD או מיישום של SaaS מחובר, התכונות אמורות להיות גלויות ברשימה הנפתחת של בונה הכללים. ניתן למצוא את שם התכונה המותאמת אישית במדריך הכתובות על-ידי שאילתת תכונה של משתמש באמצעות PowerShell וחיפוש שם התכונה. ניתן גם להשתמש באפשרות זו בעת בניית כללים בתחביר הכלל.
4. ודא שהדייר שלך מכיל את הרשיון המתאים. קבוצות דינמיות מחייבות את הדייר לכלול רשיון תכלת לספירה Premium. ניתן לגשת לרשימת התוכניות לרשיונות של הודעות מיידיות של [תכלת.](https://azure.microsoft.com/pricing/details/active-directory/) ניתן לגשת לניידות Enterprise + תוכניות רישוי אבטחה [כאן](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. ודא שהתפקיד של המשתמש היוצר את הקבוצה הדינאמית הוא מנהל מערכת כללי, כוונון מנהל מערכת, מנהל קבוצה או מנהל משתמש.
6. נא אפשר זמן לאכלוס הקבוצה. בהתאם לגודל הדייר, ייתכן שהקבוצה תימשך עד 24 שעות לאכלוס בפעם הראשונה או אחרי שינוי כללי.
7. לקבלת מידע נוסף, ראה [יצירת כללים המבוססים על תכונה עבור חברות בקבוצה דינאמית](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**אני צריך למחוק קבוצה**

1. ניתן למחוק קבוצות ממדריך הכתובות באמצעות ה-cmdlet הRemove-AzureADGroup במודול ' תכלת-Powershell '.
2. לפני שתנסה למחוק קבוצה מסונכרנת ב-תכלת AD, ודא שמחקת את כל הרשיונות שהוקצו כדי למנוע שגיאות.
3. לקבלת מידע נוסף אודות מחיקת קבוצות, ראה [מחיקת קבוצה עם רשיון מוקצה](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**עליי לשחזר קבוצה שנמחקה**

1. אם הקבוצה של Office 365 נמחקת, ניתן לשחזר אותה רק עד 30 יום לפני שתתרחש מחיקה קבועה. לאחר שנמחק לצמיתות, לא ניתן עוד לשחזר את הקבוצה. קבל מידע נוסף על שחזור קבוצות [כאן](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. פונקציונליות זו אינה נתמכת עבור קבוצות אבטחה וקבוצות תפוצה.
3. ודא שאתה מורשה לשחזר קבוצה של Office 365. מנהלי מערכת כלליים, מנהלי קבוצות, מנהלי חשבונות משתמשים, כוונון מנהלי שירות, שותפים tier1 או תמיכה של tier2, והבעלים של הקבוצה יכול להיות מסוגל לשחזר קבוצה.
4. כאשר קבוצה דינאמית נמחקת ומשוחזרת, היא נראית כקבוצה חדשה ומאוכלסת מחדש בהתאם לכלל. תהליך זה עשוי להימשך עד 24 שעות.
5. לקבלת מידע נוסף אודות שחזור קבוצה שנמחקה, ראה [שחזור קבוצה של Office 365 שנמחקה ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**תצורת מדיניות תפוגה קבוצתית**

1. פונקציונליות זו נתמכת רק עבור קבוצות Office 365, ולא עבור קבוצות אבטחה וקבוצות הפצה אינן נתמכות.
2. קביעת התצורה של מדיניות התפוגה והשימוש בה עבור קבוצות של Office 365 מחייבת רשיון של תכלת AD Premium.
3. בשלב זה, ניתן להגדיר מדיניות תפוגה אחת בלבד עבור קבוצות Office 365 בדייר.
4. רק מנהלי מערכת כלליים, מנהלי קבוצות, מנהלי משתמשים ובעלי הקבוצה יכולים להיות מסוגלים לחדש קבוצה.
5. אם פג תוקפה של קבוצה של Office 365, היא נמחקת וניתן לשחזר אותה רק עד 30 יום לפני שתתרחש מחיקה קבועה. לאחר שנמחק לצמיתות, לא ניתן עוד לשחזר את הקבוצה. קבל מידע נוסף על שחזור קבוצות [כאן](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**חידוש אוטומטי מבוסס פעילות**

פעילויות משתמש מ-SharePoint, Outlook ו-Teams יכולות להפעיל את החידוש האוטומטי של הקבוצה. פעילויות מסומנות ב-35 ימים לפני תפוגת הקבוצה. אם קיימת פעילות במהלך מחזור החיים של הקבוצה הנוכחית, הקבוצה תתחדש באופן אוטומטי והודעת דואר אלקטרוני לא תישלח לבעלים של הקבוצה.

**תזמון הודעות עבור קבוצות שפג תוקפן**

1. הודעות דואר אלקטרוני נשלחות לבעלים של קבוצת Office 365 30 יום, 15 ימים ויום אחד לפני פקיעת התוקף של הקבוצה.
2. כאשר אתה מגדיר לראשונה את התפוגה, כל הקבוצות הישנות יותר ממרווח התפוגה מוגדרות ל-35 ימים עד לפקיעת התוקף.
3. תאריך התפוגה של הקבוצה מחושב בהתבסס על תאריך החידוש של הקבוצה, ולא בהתבסס על תאריך עדכון המדיניות. אם מדיניות התפוגה מתעדכנת, תאריך התפוגה לא ישתנה.
4. לקבלת מידע נוסף, ראה [מדיניות תפוגה קבוצתית והודעות על חידוש](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) [ושחזור קבוצה של Office 365 שנמחקה ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**הרשאה ליצירת קבוצה**

ודא שאתה מורשה ליצור קבוצה חדשה. מנהלי מערכת כלליים יכולים להפוך את יצירת הקבוצה ללא זמינה בלוח תכלת או בלוח הגישה. ייתכן שתזדקק למנהל מערכת כדי ליצור את הקבוצה החדשה עבורך, או כדי להעניק לך הרשאות מתאימות.

1. [יצירת קבוצה חדשה והוספת חברים בפורטל התכלת](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [יצירת קבוצות ב-Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [ביטול יצירת קבוצות ב-Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [ניהול מי יכול ליצור קבוצות ב-Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [הפיכת הודעת הפתיחה של Office 365 ללא זמינה באמצעות Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [תפקידים מנהליים של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**ניהול הרשאות יצירת קבוצה**

1. מנהלי מערכת כלליים יכולים לנהל הרשאות יצירת קבוצה עבור אבטחה או קבוצות של Office 365 שנוצרו בפורטל ' תכלת ' או בלוח הגישה, על-ידי הגדרת **משתמשים יכולים ליצור קבוצות אבטחה בפורטלים של תכלת** או **משתמשים יכולים ליצור קבוצות של office 365 בהגדרות של פורטלי** תכלת בכל **הקבוצות > כללי (הגדרות)**.
2. באפשרותך גם להגביל את יצירת הקבוצה כדי לבחור קבוצת משתמשים אם יש לך רשיון מסוג תכלת AD P1 Premium.

**הפיכת הודעת הפתיחה ללא זמינה עבור חברים חדשים בקבוצה של Office 365**

ניתן להפוך את הודעת הפתיחה למשתמשים שנוספו לקבוצות של Office 365 לבלתי זמינה על-ידי הגדרת `UnifiedGroupWelcomeMessageEnabled` **False** ב-Powershell. קבל מידע על הגדרה זו [כאן](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













