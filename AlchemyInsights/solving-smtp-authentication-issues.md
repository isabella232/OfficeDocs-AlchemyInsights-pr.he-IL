---
title: הפיכת אימות SMTP לזמין ופתרון בעיות
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
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957209"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>הפיכת אימות SMTP לזמין ופתרון בעיות

אם ברצונך להפוך אימות SMTP לזמין עבור תיבת דואר או אם אתה מקבל שגיאת "לקוח לא מאומת", "Authentication unsuccessful", או "SmtpClientAuthentication" עם קוד 5.7.57 או 5.7.3 או 5.7.139 בעת ניסיון להעביר דואר אלקטרוני על-ידי אימות מכשיר או יישום עם Microsoft 365, בצע שלוש פעולות אלה כדי לפתור את הבעיה:

1. הפוך את [ברירות המחדל של אבטחה של Azure ללא](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) זמינות על-ידי הפעלת **ברירות מחדל של אבטחה** **ללא**.

    a. היכנס לפורטל Azure כמנהל מערכת של אבטחה, כמנהל מערכת Access כללי או כמנהל מערכת כללי.<BR/>
    b. עבור אל Azure Active Directory > **מאפיינים.**<BR/>
    c. בחר **ניהול ברירות מחדל של אבטחה**.<BR/>
    d. הגדר **את האפשרות הפוך ברירות מחדל של אבטחה לזמינות** **ללא**.<BR/>
    e. לחץ **שמור**.

2. [הפוך הגשת SMTP של לקוח](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) לזמינה בתיבת הדואר המרשית.

    a. מתוך מרכז הניהול של Microsoft 365, עבור אל **משתמשים פעילים** ובחר את המשתמש.<BR/>
    b. עבור אל הכרטיסיה דואר ותחת יישומי **דואר אלקטרוני**, בחר ניהול יישומי **דואר אלקטרוני**.<BR/>
    d. ודא **שה- SMTP מאומת** נבחר (זמין).<BR/>
    e. בחר **שמור שינויים**.<BR/>

3. [הפוך אימות רב-גורמי (MFA) ללא זמין](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) בתיבת הדואר המרשית.

    a. עבור אל מרכז הניהול של Microsoft 365, ובתפריט הניווט הימני, בחר משתמשים   >  **פעילים משתמשים**.<BR/>
    b. בחר **אימות רב-גורמי**.<BR/>
    c. בחר את המשתמש והפוך את **אימות Multi-Factor ללא זמין.**<BR/>
