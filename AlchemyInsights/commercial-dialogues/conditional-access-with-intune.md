---
title: שימוש בגישה מותנית עם כוונון
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746028"
---
# <a name="using-conditional-access-with-intune"></a>שימוש בגישה מותנית עם כוונון

שימוש בגישה מותנית עם האפשרות ' כוונון ' דורש שלושה שלבים:

- [צור מדיניות תאימות כדי להגדיר הגדרות שיש לעמוד בהן לפני שההתקן ייחשב כתואם. לדוגמה, התקן חייב לכלול pin של 6 ספרות לפחות לפני שהוא נחשב לתואם.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [צור מדיניות גישה מותנית המגדירה אילו משאבים מוגנים, ואילו תנאים דרושים לפגישה כדי לגשת למשאבים אלה. לדוגמה, התקן חייב להיות תואם לפני הגישה לדואר אלקטרוני של החברה.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [ודא שפריטי מדיניות התאימות ומדיניות גישה מותנית מיועדים לקבוצות המשתמשים הרצויות. פעולה זו עשויה לדרוש יצירת קבוצות ספציפיות של משתמשים ב-תכלת Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[קרא עוד...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
