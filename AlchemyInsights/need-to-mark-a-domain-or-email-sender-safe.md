---
title: צריך לסמן תחום או שולח דוא ל בטוח?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281149"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>צריך לסמן תחום או שולח דוא ל בטוח?

- **שימוש ברשימות שולח בטוחות אינו מומלץ מאחר** שהוא פותח את הארגון שלך לדואר זבל, phish והתקפות זיופים.
- עם זאת, אם קיימת דרישה עסקית, אנו **ממליצים** להשתמש **[בכללי זרימת דואר](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** עבור פעולה זו. ההנחיה שלנו מבטיחה אימות שולח (מוודא ששליחת קבוצת מחשבים אינה מתחזה). **הערה**: אנו לא ממליצים על ניהול תוצאות חיוביות כוזבות באמצעות רשימות שולח בטוחות, מכיוון שחריגים לסינון דואר זבל יכולים לפתוח את הארגון שלך להתקפות אבטחה. אם המשתמש שלך מקבל הודעות המסומנות באופן שגוי כדואר זבל או כדואר זבל, **[דווח למיקרוסופט על הודעות וקבצים](https://protection.office.com/reportsubmission)**.
- **יש להימנע** משולחים בטוחים ב-Outlook, רשימת שולחים מותרים, או רשימת תחומים המותרים במדיניות נגד דואר זבל, מכיוון ששולחים עוקפים את כל הודעות הזבל, הפרודיה וההגנה של פיש ואימות השולח (SPF, dkim, dkim). שיטה זו משמשת באופן הטוב ביותר לבדיקה זמנית בלבד.
