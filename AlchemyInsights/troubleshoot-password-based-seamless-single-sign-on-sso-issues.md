---
title: פתרון בעיות כניסה יחידה (SSO) מבוססת סיסמה
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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972825"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>פתרון בעיות כניסה יחידה (SSO) מבוססת סיסמה

כדי ללמוד את היסודות של SSO מבוסס-סיסמה, ראה [אימות מבוסס סיסמה באמצעות Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**קביעת תצורה של SSO מבוסס סיסמה**

1. [קביעת תצורה של כניסה יחידה מבוססת סיסמה](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - מאמר זה מפורט יותר לגבי אפשרות ה- SSO המבוססת על סיסמה. אם היישום שאתה מוסיף דורש תצורה מותאמת אישית ועלך להשתמש ב- SSO מבוסס-סיסמה, מאמר זה הוא בשבילך.
2. קביעת תצורה של כניסה יחידה המבוססת על סיסמה עבור אפליקציות [on-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - יישום Proxy תומך בכמה מצבי כניסה יחידה. כניסה מבוססת סיסמה מיועדת ליישומים המשתמשים בשילוב של שם משתמש/סיסמה לאימות. בעת קביעת התצורה של כניסה מבוססת סיסמה עבור היישום שלך, המשתמשים שלך צריכים להיכנס פעם אחת ליישום המקומי. לאחר מכן, Azure Active Directory מאחסן את פרטי הכניסה ומספק אותו באופן אוטומטי ליישום כאשר המשתמשים ניגשים אליו מרחוק.
    - כבר היית צריך לפרסם ובדקת את היישום שלך באמצעות Proxy של היישום. אם לא, בצע את השלבים המפורטים בפרסום יישומים [באמצעות Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) ולאחר מכן המשך את התצורה של SSO מבוסס-סיסמה עבור יישומים בקדם-קדם.

כדי לפתור בעיות SSO מבוסס-סיסמה, ראה פתרון בעיות כניסה יחידה [מבוססת סיסמה ב- Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
