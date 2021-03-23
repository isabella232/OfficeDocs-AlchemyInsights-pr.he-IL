---
title: בעיות בניהול משתמשים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036282"
---
# <a name="user-management-issues"></a>בעיות בניהול משתמשים

**מה קורה למשתמשים המוקצים הנוכחיים ליישום אם אני מבטל את המאפיין ' הקצאת משתמשים נדרשת ' (הגדר מאפיין זה ללא)?**

הפיכת **הקצאת משתמשים** ללא זמינה אינה משפיעה על המשתמשים המוקצים כעת. הפיכת מאפיין זה ללא זמין יאפשר לכל המשתמשים לגשת ליישום. כל המשתמשים הרשומים והמשתמשים שהוקצו לקבוצות ביישום עדיין יהיו חוקיים.

- כדי להגביל את האפליקציה שלך לקבוצה ספציפית של משתמשים, ראה- [הגבל את האפליקציה ' לספירה לכיוון תכלת ' לקבוצת משתמשים-פלטפורמת הזהות של Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- כדי להקצות משתמשים וקבוצות, ליישומים ארגוניים ב-תכלת Active Directory (תכלת לספירה), מתוך הפורטל ' תכלת ' או באמצעות PowerShell, ראה [ניהול הקצאת משתמשים עבור יישום ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- כדי להקצות הרשאות ליצירה ולניהול יישומים, ראה [הקצאת הרשאות של מנהל מערכת לניהול יישומים-תכלת לספירה | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **הסתרת יישומים ארגוניים ספציפיים ממשתמשים** -השתמש בשלבים הבאים כדי להסתיר את כל יישומי Microsoft 365 מהחלונית **היישומים שלי** . היישומים עדיין יהיו גלויים בפורטל של Office 365.

 1. היכנס לפורטל תכלת כמנהל מערכת כללי עבור מדריך הכתובות שלך. 
 2. בחר באפשרות **תכלת Active Directory**. 
 3. בחר **משתמשים**. 
 4. בחר **הגדרות משתמש**. 
 5. תחת **יישומי Enterprise**, לחץ על **נהל את האופן שבו משתמשי הקצה מפעילים ומציגים את היישומים שלהם**. 
 6. עבור **משתמשים יכולים לראות רק יישומי office 365 בפורטל של office 365**, לחץ על **כן**. 
 7. לחץ על **שמור**. 
 8. לקבלת פרטים נוספים, ראה [הסתרת יישום ארגוני מתוך חוויית המשתמש בתכלת לספירה | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- אם אתה מציע תוכנה כיישום שירות (SaaS) לארגונים רבים, באפשרותך לקבוע את התצורה של האפליקציה לקבל כניסה מכל הדיירים הפעילים של כתובות Active Directory (תכלת AD). תצורה זו נקראת "ביצוע ריבוי דיירים ביישום שלך". משתמשים בכל דייר המודע של תכלת יוכלו להיכנס לאפליקציה לאחר שתסכים להשתמש בחשבון שלו עם האפליקציה שלך. לקבלת מידע נוסף, ראה [בניית יישומים החותמים על משתמשי הודעות תכלת-פלטפורמת הזהות של Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **כיצד משתמש הקצה יכול לגשת לאפליקציה לאחר שהוא מוקצה ליישום?**

כל יישום בלהב יישום Enterprise מכיל קישור לגישה למשתמשי קצה. משתמשים יכולים גם לגשת לאפליקציה דרך פורטל **היישומים שלי** בדרך קלה.

- **רוצה לדעת אילו יישומים וסוג יישומים נמצאים בשימוש על-ידי משתמשים?**

באפשרותך להוריד דוחות כניסה עבור 30 הימים האחרונים מ- **portal.azure.com >-תכלת active directory> Signins> הורדת דוחות**.

- למד כיצד [להעניק הסכמה של מנהל מערכת של דייר רחב ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) [ולקבוע את האופן שבו משתמשי קצה מתנגדים ליישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- הכרת [אופן הפעולה של הסכמה](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [וניהול הסכמה ליישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


