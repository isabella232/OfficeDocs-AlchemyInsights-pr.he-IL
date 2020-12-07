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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583546"
---
# <a name="rbac-rules"></a>כללי RBAC

אם אתה מקבל את שגיאת ההרשאה: 

- **ללקוח עם מזהה האובייקט אין הרשאה לביצוע פעולות בטווח (קוד: AuthorizationFailed)**: כאשר אתה מנסה ליצור משאב, ודא שאתה מחובר כעת עם משתמש שהוקצה לו הרשאת כתיבה למשאב בטווח שנבחר. לדוגמה, כדי לנהל מחשבים וירטואליים בקבוצת משאבים, עליך להיות התפקיד ' [משתתף במחשב וירטואלי](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) ' בקבוצה משאבים (או בטווח האב). לקבלת רשימה של ההרשאות עבור כל תפקיד מוכלל, ראה [תפקידים מוכללים עבור משאבי התכלת](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **אין לך הרשאה ליצור בקשה לתמיכה**: כאשר אתה מנסה ליצור או לעדכן כרטיס תמיכה, ודא שאתה מחובר כעת עם משתמש שהוקצה לו תפקיד בעל הרשאת [התמיכה/](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)SupportTickets/כתיבה של Microsoft.
- **לא ניתן ליצור הקצאות תפקידים נוספות (קוד: RoleAssignmentLimitExceeded)**: כאשר אתה מנסה להקצות תפקיד, נסה לצמצם את מספר הקצאות התפקידים על-ידי הקצאת תפקידים לקבוצות במקום זאת. תכלת תומך עד **2000** הקצאות תפקידים לכל מנוי.

לקבלת פרטים נוספים על תפקידי התכלת RBAC, ראה [תפקידי rbac של התכלת](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
