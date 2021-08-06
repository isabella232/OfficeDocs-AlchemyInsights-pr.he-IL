---
title: גישת מנוי
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999241"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>לא ניתן להיכנס ל- Azure עקב בעיות בדפדפן (הדפדפן ננתק, ממשיך להסתובב, אינו נטען וכו')

ייתכן שאתה מושפע מהתנתקות. בדוק אם תם התנתקות: מצב [תקינות Azure](https://status.azure.com/status/history/).

צא מכל הפעלות Azure הפעילות. התחל מצב בסתר או באופן פרטי של דפדפן האינטרנט שלך.

באפשרותך גם לנסות לרענן דפדפן, להשתמש בדפדפן אחר, למחוק קבצי Cookie של מטמון אם לעיל אינו פועל.

קבל מידע נוסף: [פתרון בעיות כניסה](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**לא ניתן לגשת למנויים**

בפורטל [Azure,](https://portal.azure.com/)ודא שמדריך הכתובות הנכון של Azure נבחר מהחשבון בחלק השמאלי העליון.

במרכז [חשבון Azure](https://account.windowsazure.com/Subscriptions), ודא אם החשבון המשמש הוא מנהל החשבון.

מידע נוסף: [פתרון בעיות לא נמצאו מנויים](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**לא ניתן לגשת להיסטוריית חיובים**

מנהל החשבון צריך לוודא שהמשתמש ניגש לפרטי החיוב נוסף ב- Azure Active directory כמשתמש אורח: [הוספה או מחיקה של משתמש חדש.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

לאחר מכן, המשתמש צריך לקבל תפקיד מנהל מערכת כללי: [הקצאת תפקיד למשתמשים](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

פרסם זאת, המשתמש יכול לקבל גישת חיוב באמצעות מדיניות RBAC: [הענק גישה לחיוב](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**מסמכים מומלצים**

-   [איני מצליח להיכנס כדי לנהל את מנוי Azure שלי](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)