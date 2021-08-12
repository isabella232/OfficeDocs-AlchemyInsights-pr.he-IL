---
title: כיצד להוסיף ולנהל מנהלי מערכת - שלבים מומלצים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963788"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>כיצד להוסיף ולנהל מנהלי מערכת - שלבים מומלצים

בהתבסס על תיאור הבעיה שלך, מצאנו פתרון בשבילך. רוב הלקוחות הצליחו לפתור את הבעיה עצמם לאחר ביצוע התיעוד שלנו.

**עריכת מנהל המנוי או מנהל שותף**

- מנהל החשבון יכול לערוך את שני התפקידים בעוד שמנהל המנוי יכול לשנות רק מנהלים עמיתים בפורטל [Azure](https://ms.portal.azure.com/#home).
- [הוספה או שינוי של מנהלי מנוי Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**עדכון מנהל המנוי או Co-Administrator עבור מנויים פנימיים (AIRS)**

מנהל השירות או מנהל המערכת ה עמיתים יכולים לבצע פעולה זו בשירות עצמי באמצעות השלבים הבאים:

1. היכנס לפורטל [Azure ולחץ](https://ms.portal.azure.com/#home) על **ניהול עלות + חיוב** בלהב הימני.
2. לחץ על פריט השורה עם המנוי שלך. פעולה זו פותחת את 'מבט כולל' עבור המנוי שלך.
3. בלהב **המנוי,** לחץ **על מאפיינים**. 
4. לחץ על **לחצן ניהול** שירות.
5. הזן את הדואר האלקטרוני של המשתמש שברצונך להגדיר כמנהל שירות ולחץ על **אישור**.

**הוספה/שינוי/הסרה של מנהל עמית**

1. היכנס לפורטל [Azure](https://ms.portal.azure.com/#home) כמנהל שירות.
2. פתח [מנויים](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ובחר מנוי. (ניתן להקצות מנהלי מערכת עמיתים רק בטווח המנוי.)
3. נווט **אל Access (IAM)** מנהלי מערכת קלאסיים הוסף הוסף מנהל שותף כדי לפתוח את החלונית הוסף מנהל מערכת שותף (אם האפשרות הוסף מנהל עמית אינה זמינה, היא מציינת כי אין  >    >    >   לך הרשאות). 
4. בחר את המשתמש שברצונך להוסיף ולחץ על **הוסף**.

**למידע נוסף:**
- [הוספת מנהל שותף](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [הסרת מנהל מערכת שותף](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [שינוי מנהל השירות](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [הצגת מנהל החשבון](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [ניהול גישה באמצעות פורטל RBAC ו- Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**הוספה/מחיקה של משתמשים באמצעות Azure Active Directory (AD)**

באפשרותך להוסיף משתמשים חדשים או למחוק משתמשים קיימים מארגון Azure Active Directory (Azure AD) שלך:

1. כדי להוסיף משתמש חדש, היכנס [לפורטל Azure](https://ms.portal.azure.com/#home) כמנהל משתמש עבור הארגון.
2. בחר **Azure Active Directory**, בחר **משתמשים** ולאחר מכן לחץ על **משתמש חדש.**
3. בדף **משתמש,** מלא את המידע הדרוש. לחץ **על צור**. המשתמש נוצר ונוסף לדייר Azure AD שלך.

**קבל מידע נוסף**:

- [הוספת משתמש חדש](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [מחיקת משתמש](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [הוספה או עדכון של פרטי פרופיל של משתמש באמצעות Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**מסמכים מומלצים**

- [מהו בקרת גישה מבוססת תפקידים (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [הבנת התפקידים השונים ב- Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [הרשאות תפקיד מנהל מערכת ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [ערכת לימוד: הענק גישה עבור משתמש באמצעות RBAC ופורטל Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [פתרון בעיות של RBAC ב- Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [ארגון המשאבים שלך באמצעות קבוצות ניהול Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [כיצד לבקש עותק של חשבונית Azure באמצעות דואר אלקטרוני](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [כיצד להוסיף, לעדכן או להסיר כרטיס אשראי או חיוב מ- Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [ניהול (הפעלה מחדש/ביטול/החלפה) מנוי](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



