---
title: פתרון בעיות של כניסה יחידה (SSO) חלקה מבוססת סיסמה
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714769"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>פתרון בעיות של כניסה יחידה (SSO) חלקה מבוססת סיסמה

כדי ללמוד את היסודות של SSO מבוסס סיסמה, ראה [אימות מבוסס סיסמה עם תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**קביעת תצורה של SSO מבוסס סיסמה**

1. [קביעת התצורה של כניסה יחידה מבוססת סיסמה-מאמר](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) זה מתקבלת לפרטים נוספים אודות האפשרות SSO מבוססת סיסמה. אם היישום שאתה מוסיף דורש תצורה מותאמת אישית ועליך להשתמש ב-SSO מבוסס סיסמה, מאמר זה מיועד לך.
2. [קביעת התצורה של כניסה יחידה מבוססת סיסמה עבור יישומים ב-פרם](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -Proxy של יישום תומך בכמה מצבי כניסה יחידה. כניסה מבוססת סיסמה מיועדת ליישומים המשתמשים בשילוב של שם משתמש/סיסמה לצורך אימות. בעת קביעת התצורה של כניסה מבוססת סיסמה עבור היישום, המשתמשים שלך צריכים להיכנס ליישום המקומי פעם אחת. לאחר מכן, תכלת Active Directory מאחסן את מידע הכניסה ומספק אותו באופן אוטומטי ליישום כאשר המשתמשים שלך ניגשים אליו מרחוק.
    - כבר היית אמור לפרסם ולבדוק את האפליקציה באמצעות Proxy של יישומים. אם לא, בצע את השלבים המפורטים [ביישומי פרסום באמצעות האפליקציה ' שימוש ב-תכלת לספירה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) ' ולאחר מכן המשך בקביעת התצורה של SSO מבוסס-סיסמה עבור אפליקציות של ה-פרם

כדי לפתור בעיות ב-SSO מבוסס סיסמה, ראה [פתרון בעיות בכניסה יחידה מבוססת סיסמה בתכלת לספירה](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
