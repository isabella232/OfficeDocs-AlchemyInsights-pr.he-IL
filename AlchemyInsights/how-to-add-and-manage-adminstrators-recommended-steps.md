---
title: כיצד להוסיף ולנהל מנהלים-שלבים מומלצים
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755836"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>כיצד להוסיף ולנהל מנהלים-שלבים מומלצים

בהתבסס על תיאור הבעיה שלך, מצאנו פתרון עבורך. רוב הלקוחות הצליחו לפתור את הבעיה שלהם בעצמם לאחר ביצוע התיעוד שלנו.

**עריכת מנהל המנוי או מנהל מערכת משותף**

- מנהל החשבון יכול לערוך את שני התפקידים בעוד שמנהל המנוי יכול לשנות רק מנהלים משותפים [בפורטל התכלת](https://ms.portal.azure.com/#home).
- [הוספה או שינוי של מנהלי מנויים של תכלת](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**עדכון מנהל המנוי או Co-Administrator עבור מנויים פנימיים (משודרים)**

מנהל השירות או מנהל המערכת המשותף יכולים לשרת פעולה זו באופן עצמאי באמצעות השלבים הבאים:

1. היכנס [לפורטל תכלת](https://ms.portal.azure.com/#home) ולחץ על **ניהול עלות + חיוב** בלהב הימני.
2. לחץ על פריט השורה עם המנוי שלך. פעולה זו פותחת את הסקירה עבור המנוי שלך.
3. בלהב **המנוי** , לחץ על **מאפיינים**. 
4. לחץ על לחצן **מנהל השירות** .
5. הזן את הודעת הדואר האלקטרוני של המשתמש שברצונך להגדיר כמנהל שירות ולחץ על **אישור**.

**הוספה/שינוי/הסרה של מנהל מערכת משותף**

1. היכנס [לפורטל התכלת](https://ms.portal.azure.com/#home) כמנהל שירות.
2. פתח [מנויים](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ובחר מנוי. (ניתן להקצות את adminstrators בטווח המנוי בלבד).
3. נווט אל   >  **מנהלי מערכת קלאסיים** של בקרת גישה (יאם)  >    >  הוסף **הוסף מנהל מערכת** כדי לפתוח את החלונית **הוספת מנהל משותף** (אם האפשרות הוסף מנהל משותף אינה זמינה, היא מציינת שאין לך הרשאות).
4. בחר את המשתמש שברצונך להוסיף ולחץ על **הוסף**.

**למד עוד:**
- [הוספת מנהל מערכת משותף](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [הסרת מנהל מערכת משותף](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [שינוי מנהל השירות](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [הצגת מנהל החשבון](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [ניהול גישה באמצעות הפורטל של RBAC ותכלת](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**הוספה/מחיקה של משתמשים באמצעות ' תכלת Active Directory ' (AD)**

באפשרותך להוסיף משתמשים חדשים או למחוק משתמשים קיימים מארגון תכלת Active Directory (תכלת לספירה):

1. כדי להוסיף משתמש חדש, היכנס [לפורטל תכלת](https://ms.portal.azure.com/#home) כמנהל משתמש עבור הארגון.
2. בחר באפשרות **תכלת Active Directory**, בחר **משתמשים** ולאחר מכן לחץ על **משתמש חדש**.
3. בדף **המשתמש** , מלא את המידע הנדרש. לחץ על **צור**. המשתמש נוצר ונוסף לדייר המודע של תכלת.

**מידע נוסף**:

- [הוספת משתמש חדש](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [מחיקת משתמש](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [הוספה או עדכון של פרטי פרופיל של משתמש באמצעות ' תכלת Active Directory '](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**מסמכים מומלצים**

- [מהו בקרת גישה מבוססת תפקידים (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [הבנת התפקידים השונים בתכלת](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [הרשאות תפקיד מנהל מערכת ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [ערכת לימוד: הענקת גישה למשתמש באמצעות RBAC ופורטל תכלת](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [פתרון בעיות ב-RBAC בתכלת](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [ארגון משאבים עם קבוצות ניהול של ' תכלת '](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [כיצד לבקש עותק של חשבונית התכלת באמצעות דואר אלקטרוני](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [כיצד להוסיף, לעדכן או להסיר כרטיס אשראי או חיוב מתכלת](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [ניהול (הפעלה מחדש של מנוי/ביטול/מעבר)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



