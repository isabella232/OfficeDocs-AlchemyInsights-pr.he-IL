---
title: ייבוא וייצוא מ-קטרת
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036125"
---
# <a name="import-and-export-from-yammer"></a>ייבוא וייצוא מ-קטרת

**ייבוא**

אפשרויות ייבוא משתמשים משתנות בהתאם לשאלה אם רשת קטרת שלך נמצאת [במצב מקורי עבור Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)או לא.

- **מצב שאינו מקורי**: ניתן לייבא משתמשים לקבוצות באמצעות [הוסף מפנקס הכתובות](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (מגבלה למשתמשי 100) בתוך הגדרות קבוצה, או ברשת באמצעות [עדכון בצובר](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) בתוך מנהל הרשת.
- **מצב מקורי**: יש לבצע את החברות בקבוצה ואת פעולות החברות ברשת [מפורטל הניהול של Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [מפורטל תכלת לספירה](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), או באמצעות אפשרות אחרת של כרטיס לספירה. לרשתות במצב מקורי אין עוד גישה לעדכון בצובר ולתכונות מדור קודם אחר.

> [!IMPORTANT]
> קטרת מעולם לא תמך בייבוא תוכן מתוך מנהל הרשת גם כאשר נעשה שימוש בתכונת ייצוא הנתונים ברשת אחרת. ניתן לפרסם מחדש תוכן על-ידי פתרונות שותפים או ממשקי Api של קטרת REST.

**ייצוא**

[ייצוא נתוני רשת בתוך מנהל הרשת](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) מאפשר ייצוא תוכן מרשתות קטרת, כולל הודעות וקבצים. קבצים מצורפים יכולים להיות גדולים מאוד ולגרום לייצוא להשלים זמן משמעותי. מומלץ לייצא רשתות פעילות באמצעות ה- [API של ייצוא הנתונים](https://developer.yammer.com/docs/data-export-api) בגושים לפי יום או שבוע. התמיכה של Microsoft אינה מספקת קבצי script מותאמים אישית למטרה זו.

[ייצוא GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) נפרד קיים כדי לייצא תוכן עבור משתמש בודד.