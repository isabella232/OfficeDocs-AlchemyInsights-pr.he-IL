---
title: שימוש ב- Access עם Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005775"
---
# <a name="using-conditional-access-with-intune"></a>שימוש ב- Access עם Intune

שימוש ב- Access עם Intune דורש 3 שלבים:

- [צור מדיניות תאימות כדי להגדיר הגדרות שיש לבצע לפני שהמכשיר נחשב לתואם. לדוגמה, למכשיר חייב להיות מספר זיהוי של לפחות 6 ספרות לפני שהוא נחשב לתואם.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [צור מדיניות Access מותנות המגדירה אילו משאבים מוגנים, ואל אילו תנאים יש לגשת למשאבים אלה. לדוגמה, מכשיר חייב להיות תואם לפני גישה לדואר אלקטרוני ארגוני.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [ודא שמדיניות תאימות ומדיניות Access מותנה ממוקדים לקבוצות המשתמשים הרצויות. פעולה זו עשויה לדרוש יצירת קבוצות ספציפיות של משתמשים ב- Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[קרא עוד...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
