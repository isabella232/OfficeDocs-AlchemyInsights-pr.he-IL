---
title: 451 4.7.0 שגיאת שרת זמני. נסה שוב מאוחר יותר. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812580"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 שגיאת שרת זמני. נסה שוב מאוחר יותר. PRX4

ייתכן שתתמודד עם בעיה בעת שליחת דואר אלקטרוני באמצעות Smarthost "smtp.office365.com" באמצעות שיטת שליחת לקוח SMTP ותקבל את השגיאה: "451 4.7.0 שגיאת שרת זמנית. נסה שוב מאוחר יותר. PRX4 הוא בעיקר זמני". 

ודא שאתה לא משתמש בתיבת דואר משותפת עבור שליחת לקוח SMTP, כאשר שיטת השליחה של לקוח SMTP דורשת תיבת דואר עם רשיון לשליחת דואר דרך. עם זאת, אם אינך משתמש בתיבת דואר משותפת והבעיה נמשכת, בדוק את הפעולות הבאות:

1. הפוך הגשת SMTP של לקוח לזמינה בתיבת הדואר המרשית המשמשת אותך על-ידי הפעלת פקודה זו של PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    או

    1. עבור אל מרכז הניהול של Microsoft 365 > **פעילים** ובחר את המשתמש.
    1. עבור אל הכרטיסיה דואר > **דואר אלקטרוני >** ניהול יישומי דואר **אלקטרוני**. 
    1. ודא שההגדרה **אימות SMTP** נבחרה (זמינה).
    1. בחר **שמור שינויים**.
    
    כדי להפוך אימות SMTP לזמין עבור ארגון שלם, הפעל פקודה זו:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **הערה:** מטעמי אבטחה, מומלץ להפוך אימות SMTP לזמין רק עבור תיבת הדואר המשמשת אותך. הגדרת רמת המשתמש עוקפת את הגדרת רמת הארגון.

2. הפוך את ברירות המחדל של Azure Security ללא זמינות על-ידי הפעלת **ברירות מחדל של אבטחה** **ללא**:

    1. היכנס לפורטל Azure כמנהל אבטחה, כמנהל מערכת Access כללי או כמנהל מערכת כללי.
    1. עבור אל Azure Active Directory >**  מאפיינים** ובחר ניהול **ברירות מחדל של אבטחה**.
    1. הגדר את הלחצן **הדו-מצבי הפוך ברירות מחדל של אבטחה** לזמינות **ללא**.
    1. לחץ **שמור**.

3. הפוך אימות רב-גורמי (MFA) ללא זמין בתיבת הדואר המרשית המשמשת אותך.

    1. עבור אל מרכז הניהול של Microsoft 365, ובתפריט הניווט הימני, בחר משתמשים  >  **פעילים משתמשים**.
    1. בדף משתמשים **פעילים,** בחר אימות **רב-גורמי**.
    1. בחר את המשתמש והשבת אימות **רב-גורמי**.

