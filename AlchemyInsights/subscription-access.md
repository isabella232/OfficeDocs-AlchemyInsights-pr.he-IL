---
title: גישה למנוי
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807433"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>לא ניתן להיכנס לתכלת עקב בעיות בדפדפן (הדפדפן נתקע, ממשיך להסתובב, אינו נטען וכדומה).

ייתכן שאתה מושפע מהנפילה. בדוק אם קיימת הפסקת פעולה מתמשכת: [מצבי תקינות התכלת](https://status.azure.com/status/history/).

צא מכל ההפעלות הפעילות של ' תכלת '. התחל מצב של דפדפן האינטרנט באופן פרטי או בעילום שם.

באפשרותך גם לנסות לרענן דפדפן, להשתמש בדפדפן אחר, למחוק קבצי cookie של מטמון אם לעיל אינו פועל.

מידע נוסף: [פתרון בעיות כניסה](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**אין אפשרות לגשת למנויים**

בפורטל ' [תכלת](https://portal.azure.com/)', ודא שהאפשרות ' התכלת הנכון ' נבחרה מהחשבון בחלק השמאלי העליון.

במרכז [החשבון של תכלת](https://account.windowsazure.com/Subscriptions), ודא שהחשבון משמש כמנהל החשבון.

מידע נוסף: [פתרון בעיות לא נמצאו מנויים](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**לא ניתן לגשת להיסטוריית החיוב**

מנהל החשבונות צריך לוודא שהמשתמש הניגש לפרטי החיוב מתווסף ל-תכלת Active directory כמשתמש אורח: [הוספה או מחיקה של משתמש חדש](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

לאחר מכן, המשתמש צריך לקבל תפקיד מנהל מערכת כללי: [הקצה תפקיד למשתמשים](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

פרסם זאת, המשתמש יכול לקבל גישה לחיוב באמצעות מדיניות RBAC: [הענקת גישה לחיוב](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**מסמכים מומלצים**

-   [איני מצליח להיכנס כדי לנהל את מנוי התכלת שלי](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)