---
title: 'תפקידי RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923132"
---
# <a name="rbac-rules"></a>כללי RBAC

אם אתה מקבל את שגיאת ההרשאה: 

- ללקוח עם מזהה אובייקט אין הרשאה לבצע פעולה מעל **טווח (קוד: AuthorizationFailed)**: בעת ניסיון ליצור משאב, ודא שאתה מחובר כעת עם משתמש שהוקצה לו תפקיד בעל הרשאת כתיבה למשאב בטווח שנבחר. לדוגמה, כדי לנהל מחשבים וירטואליים בקבוצת משאבים, התפקיד ['משתתף מחשב](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) וירטואלי' צריך להיות בקבוצת המשאבים (או בטווח האב). לקבלת רשימה של ההרשאות עבור כל תפקיד מוכלל, ראה [תפקידים מוכללים עבור משאבי Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **אין לך הרשאה** ליצור בקשת תמיכה : בעת ניסיון ליצור או לעדכן כרטיס תמיכה, ודא שאתה מחובר כעת עם משתמש שהוקצה לו תפקיד בעל ההרשאה Microsoft.Support/supportTickets/write, כגון [משתתף בקשת תמיכה.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- **לא ניתן ליצור הקצאות תפקידים נוספות (קוד: RoleAssignmentLimitExceed)**: כאשר אתה מנסה להקצות תפקיד, נסה להקטין את מספר הקצאות התפקידים על-ידי הקצאת תפקידים לקבוצות במקום זאת. Azure תומך במטלות תפקיד של עד **2000** לכל מנוי.

לקבלת פרטים נוספים על תפקידי Azure RBAC, ראה [תפקידי Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
