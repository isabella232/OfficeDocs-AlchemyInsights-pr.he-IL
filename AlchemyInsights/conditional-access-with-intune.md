---
title: גישה מותנית עם כוונון
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807660"
---
# <a name="conditional-access-with-intune"></a>גישה מותנית עם כוונון

שימוש  **בגישה מותנית**  עם האפשרות ' כוונון ' דורש שלושה שלבים:

- צור  **מדיניות תאימות**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) כדי להגדיר הגדרות שיש לעמוד בהן לפני שההתקן ייחשב כתואם. לדוגמה, התקן חייב לכלול pin של 6 ספרות לפחות לפני שהוא נחשב לתואם.
- צור **מדיניות גישה מותנית**  המגדירה אילו משאבים מוגנים, ואילו תנאים דרושים לפגישה כדי לגשת למשאבים אלה.  [לדוגמה,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  התקן חייב להיות תואם לפני הגישה לדואר אלקטרוני של החברה.
- ודא **שפריטי מדיניות התאימות**  **ומדיניות גישה מותנית**  מיועדים לקבוצות המשתמשים הרצויות. פעולה זו עשויה לדרוש יצירת קבוצות ספציפיות של משתמשים ב-תכלת Active Directory.

**קישורים שימושיים:**

[מבט כולל על תאימות מכשירים](https://docs.microsoft.com/intune/device-compliance-get-started)

[פתרון בעיות ב-CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[מדיניות פתרון בעיות](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

כדי להגן על דואר אלקטרוני (Exchange online) מ-access על-ידי מכשירים שאינם תואמים, יש לעקוב אחר שני המסמכים:

1. [הגנה על גישה לדואר אלקטרוני ממכשירים המשתמשים במלווים](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [הגנה על גישה לדואר אלקטרוני ממכשירים באמצעות לקוחות אימות מודרניים כגון Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)